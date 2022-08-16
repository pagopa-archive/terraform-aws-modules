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
| [aws_customer_gateway.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/customer_gateway) | resource |
| [aws_vpn_connection.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpn_connection) | resource |
| [aws_vpn_gateway.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpn_gateway) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_connection_tunnel"></a> [aws\_connection\_tunnel](#input\_aws\_connection\_tunnel) | vpn connection tunnel configs | <pre>object({<br>    ike                = list(string)<br>    dh_group           = list(number)<br>    enc_alg            = list(string)<br>    int_alg            = list(string)<br>    dpd_timeout_action = string<br>    startup_action     = string<br>  })</pre> | n/a | yes |
| <a name="input_aws_vpn_connection_type"></a> [aws\_vpn\_connection\_type](#input\_aws\_vpn\_connection\_type) | aws vpn connection type | `string` | `"ipsec.1"` | no |
| <a name="input_customer_gateway"></a> [customer\_gateway](#input\_customer\_gateway) | customer gateway properties | <pre>object({<br>    ip = string<br>  })</pre> | `null` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | A map of tags, each pair. | `map(string)` | `null` | no |
| <a name="input_vpc_id"></a> [vpc\_id](#input\_vpc\_id) | The vpc id | `string` | n/a | yes |

## Outputs

No outputs.
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
