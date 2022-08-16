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
| [aws_iam_policy.aws_kinesis_firehose_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy_attachment.aws_kinesis_firehose_policy-attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy_attachment) | resource |
| [aws_iam_role.firehose_role](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_kinesis_firehose_delivery_stream.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/kinesis_firehose_delivery_stream) | resource |
| [aws_iam_policy_document.firehose_put_role_template](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_bucket_arn"></a> [bucket\_arn](#input\_bucket\_arn) | Destination bucket ARN | `string` | `null` | no |
| <a name="input_firehose_extended_s3_configurations"></a> [firehose\_extended\_s3\_configurations](#input\_firehose\_extended\_s3\_configurations) | Extended S3 configurations | `map(string)` | <pre>{<br>  "bucket_arn": null,<br>  "buffer_interval": 60,<br>  "buffer_size": 5,<br>  "cloudwatch_enabled": false,<br>  "cloudwatch_log_group": null,<br>  "cloudwatch_log_stream_name": null,<br>  "error_output_prefix": null,<br>  "kms_key_arn": null,<br>  "prefix": null<br>}</pre> | no |
| <a name="input_firehose_iam_policy"></a> [firehose\_iam\_policy](#input\_firehose\_iam\_policy) | Firehose IAM policy | `string` | `null` | no |
| <a name="input_firehose_name"></a> [firehose\_name](#input\_firehose\_name) | The name of the delivery stream. | `string` | `null` | no |
| <a name="input_firehose_server_side_encryption"></a> [firehose\_server\_side\_encryption](#input\_firehose\_server\_side\_encryption) | Server side encryption configuration | `map(string)` | <pre>{<br>  "enabled": false,<br>  "key_arn": null,<br>  "key_type": null<br>}</pre> | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_arn"></a> [arn](#output\_arn) | n/a |
| <a name="output_id"></a> [id](#output\_id) | n/a |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
