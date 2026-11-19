## Usage

```hcl
module "bucket" {
  source = "git::https://github.com/rafalmasiarek/terraform-cloudflare-r2-backend-bootstrap.git//modules/r2_bucket?ref=v0.1.0"

  account_id    = var.account_id
  name          = "my-tfstate"
  location      = "weur"
  storage_class = "Standard"
}
```

This module is normally not called directly - it's an internal building
block for the root [terraform-cloudflare-r2-backend-bootstrap](../../) module.
