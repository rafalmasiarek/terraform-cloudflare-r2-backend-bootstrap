## Terraform Reference



### Requirements

No requirements.

### Modules

| Name | Source | Version |
| ---- | ------ | ------- |
| <a name="module_bucket"></a> [bucket](#module\_bucket) | git::https://github.com/rafalmasiarek/terraform-cloudflare-r2-bucket.git | v0.2.0 |

### Resources

No resources.

### Inputs

| Name | Description | Type | Default | Required |
| ---- | ----------- | ---- | ------- | :------: |
| <a name="input_account_id"></a> [account\_id](#input\_account\_id) | Cloudflare account ID. | `string` | n/a | yes |
| <a name="input_bucket_lifecycle"></a> [bucket\_lifecycle](#input\_bucket\_lifecycle) | R2 bucket lifecycle configuration. | `any` | `null` | no |
| <a name="input_cors"></a> [cors](#input\_cors) | R2 bucket CORS configuration. | `any` | `null` | no |
| <a name="input_custom_domains"></a> [custom\_domains](#input\_custom\_domains) | R2 custom domains configuration. | `any` | `{}` | no |
| <a name="input_event_notifications"></a> [event\_notifications](#input\_event\_notifications) | R2 event notifications configuration. | `any` | `{}` | no |
| <a name="input_location"></a> [location](#input\_location) | R2 bucket location. | `string` | `null` | no |
| <a name="input_lock"></a> [lock](#input\_lock) | R2 bucket lock configuration. | `any` | `null` | no |
| <a name="input_managed_domain"></a> [managed\_domain](#input\_managed\_domain) | R2 managed domain configuration. | `any` | `null` | no |
| <a name="input_name"></a> [name](#input\_name) | R2 bucket name. | `string` | n/a | yes |
| <a name="input_sippy"></a> [sippy](#input\_sippy) | R2 Sippy configuration. | `any` | `null` | no |
| <a name="input_storage_class"></a> [storage\_class](#input\_storage\_class) | R2 bucket storage class. | `string` | `null` | no |

### Outputs

| Name | Description |
| ---- | ----------- |
| <a name="output_bucket"></a> [bucket](#output\_bucket) | R2 bucket object returned by the wrapped module. |
| <a name="output_bucket_id"></a> [bucket\_id](#output\_bucket\_id) | R2 bucket ID. |
| <a name="output_bucket_location"></a> [bucket\_location](#output\_bucket\_location) | R2 bucket location. |
| <a name="output_bucket_name"></a> [bucket\_name](#output\_bucket\_name) | R2 bucket name. |
| <a name="output_bucket_storage_class"></a> [bucket\_storage\_class](#output\_bucket\_storage\_class) | R2 bucket storage class. |