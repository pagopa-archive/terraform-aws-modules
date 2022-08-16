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
| [aws_iam_access_key.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_access_key) | resource |
| [aws_iam_user.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user) | resource |
| [aws_iam_user_policy.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user_policy) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_ses_user"></a> [ses\_user](#input\_ses\_user) | User name of SES user | `string` | `"ses-user"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_aws_iam_access_key"></a> [aws\_iam\_access\_key](#output\_aws\_iam\_access\_key) | n/a |
| <a name="output_aws_iam_access_key_id"></a> [aws\_iam\_access\_key\_id](#output\_aws\_iam\_access\_key\_id) | n/a |
| <a name="output_aws_iam_smtp_password"></a> [aws\_iam\_smtp\_password](#output\_aws\_iam\_smtp\_password) | n/a |
| <a name="output_aws_iam_smtp_user"></a> [aws\_iam\_smtp\_user](#output\_aws\_iam\_smtp\_user) | n/a |
| <a name="output_aws_iam_user_name"></a> [aws\_iam\_user\_name](#output\_aws\_iam\_user\_name) | n/a |
| <a name="output_aws_iam_user_name_arn"></a> [aws\_iam\_user\_name\_arn](#output\_aws\_iam\_user\_name\_arn) | n/a |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
