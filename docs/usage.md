## Usage

```hcl
module "backend" {
  source = "git::https://github.com/rafalmasiarek/terraform-cloudflare-r2-backend-bootstrap.git?ref=v0.1.0"

  account_id    = var.account_id
  account_alias = var.account_alias
  environment   = var.environment

  name_prefix    = var.name_prefix
  bucket_purpose = "tfstate"

  state_key     = var.state_key
  storage_class = "Standard"

  backup_enabled              = true
  backup_uses_separate_bucket = true
  backup_trigger              = "event"

  backup_storage_class = "Standard"
  backup_prefix        = "snapshots"
  backup_source_suffix = ".tfstate"

  backup_retention_days           = 90
  enable_backup_lock              = true
  backup_min_lock_days             = 14
  enable_backup_dead_letter_queue = true
}
```

See `examples/complete`, `examples/event-internal-bucket`, and
`examples/scheduled-internal-bucket` for full, runnable variants.
