<!-- markdownlint-disable -->
<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.1.0 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | <= 4.26.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 4.26.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_key_pair.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/key_pair) | resource |
| [aws_secretsmanager_secret.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/secretsmanager_secret) | resource |
| [aws_secretsmanager_secret_version.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/secretsmanager_secret_version) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | n/a | `string` | n/a | yes |
| <a name="input_environment"></a> [environment](#input\_environment) | The name of the environment. | `string` | n/a | yes |
| <a name="input_key_name"></a> [key\_name](#input\_key\_name) | The name of the pulic key | `string` | n/a | yes |
| <a name="input_private_key_path_openssh"></a> [private\_key\_path\_openssh](#input\_private\_key\_path\_openssh) | Private key path (generate it with ssh-keygen) | `any` | n/a | yes |
| <a name="input_public_key_path_openssh"></a> [public\_key\_path\_openssh](#input\_public\_key\_path\_openssh) | Public key path (generate it with ssh-keygen) | `any` | n/a | yes |
| <a name="input_secret_key_name"></a> [secret\_key\_name](#input\_secret\_key\_name) | The name of the key within the secret | `string` | n/a | yes |
| <a name="input_secret_name"></a> [secret\_name](#input\_secret\_name) | The secret manager secret name | `string` | n/a | yes |
| <a name="input_tags"></a> [tags](#input\_tags) | A map of tags, each pair. | `map(string)` | `null` | no |
| <a name="input_version_stage"></a> [version\_stage](#input\_version\_stage) | Specifies the secret version that you want to retrieve by the staging label attached to the version. | `string` | `"AWSCURRENT"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_id"></a> [id](#output\_id) | n/a |
| <a name="output_key_name"></a> [key\_name](#output\_key\_name) | n/a |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
