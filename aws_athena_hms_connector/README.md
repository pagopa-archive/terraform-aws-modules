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
| [aws_iam_policy.aws_lambda_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy_attachment.aws_lambda_policy_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy_attachment) | resource |
| [aws_iam_role.iam_for_lambda](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_lambda_function.test_lambda](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_deployment_s3_location"></a> [deployment\_s3\_location](#input\_deployment\_s3\_location) | Deployment references | `map(string)` | <pre>{<br>  "s3_bucket": null,<br>  "s3_key": null,<br>  "s3_object_version": null<br>}</pre> | no |
| <a name="input_function_env"></a> [function\_env](#input\_function\_env) | Environment variables | `map(string)` | `null` | no |
| <a name="input_function_handler"></a> [function\_handler](#input\_function\_handler) | Lambda function handler | `string` | `null` | no |
| <a name="input_function_memory_size"></a> [function\_memory\_size](#input\_function\_memory\_size) | Memory size | `number` | `512` | no |
| <a name="input_function_name"></a> [function\_name](#input\_function\_name) | Lambda function name | `string` | `null` | no |
| <a name="input_function_policy"></a> [function\_policy](#input\_function\_policy) | Lambda function policy document | `string` | `null` | no |
| <a name="input_function_runtime"></a> [function\_runtime](#input\_function\_runtime) | Lambda function runtime | `string` | `null` | no |
| <a name="input_function_vpc_config"></a> [function\_vpc\_config](#input\_function\_vpc\_config) | VPC config | `map(list(string))` | <pre>{<br>  "security_group_ids": null,<br>  "subnet_ids": null<br>}</pre> | no |

## Outputs

No outputs.
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
