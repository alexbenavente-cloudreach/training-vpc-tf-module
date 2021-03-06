# training-vpc-tf-module
<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 2.7.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 2.7.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_eip.nat_eip](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_internet_gateway.igw](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway) | resource |
| [aws_nat_gateway.nat_gw](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) | resource |
| [aws_route_table.internet_route_table](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table.nat_route_table](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table_association.internet_route_table_association_data_a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.internet_route_table_association_data_b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.internet_route_table_association_private_a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.internet_route_table_association_private_b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.internet_route_table_association_public_a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.internet_route_table_association_public_b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_subnet.data_a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.data_b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.private_a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.private_b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_vpc.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_data_a_cidr"></a> [data\_a\_cidr](#input\_data\_a\_cidr) | The Data subnet CIDR for AZ a | `string` | n/a | yes |
| <a name="input_data_b_cidr"></a> [data\_b\_cidr](#input\_data\_b\_cidr) | The Data subnet CIDR for AZ b | `string` | n/a | yes |
| <a name="input_private_a_cidr"></a> [private\_a\_cidr](#input\_private\_a\_cidr) | The Private subnet CIDR for AZ a | `string` | n/a | yes |
| <a name="input_private_b_cidr"></a> [private\_b\_cidr](#input\_private\_b\_cidr) | The Private subnet CIDR for AZ b | `string` | n/a | yes |
| <a name="input_project_name"></a> [project\_name](#input\_project\_name) | The prefeix name of the project | `string` | n/a | yes |
| <a name="input_public_a_cidr"></a> [public\_a\_cidr](#input\_public\_a\_cidr) | The Public subnet CIDR for AZ a | `string` | n/a | yes |
| <a name="input_public_b_cidr"></a> [public\_b\_cidr](#input\_public\_b\_cidr) | The Public subnet CIDR for AZ b | `string` | n/a | yes |
| <a name="input_region_name"></a> [region\_name](#input\_region\_name) | The name of the region | `string` | n/a | yes |
| <a name="input_vpc_cidr"></a> [vpc\_cidr](#input\_vpc\_cidr) | The VPC CIDR | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_data_subnet_a_id"></a> [data\_subnet\_a\_id](#output\_data\_subnet\_a\_id) | n/a |
| <a name="output_data_subnet_b_id"></a> [data\_subnet\_b\_id](#output\_data\_subnet\_b\_id) | n/a |
| <a name="output_private_subnet_a_id"></a> [private\_subnet\_a\_id](#output\_private\_subnet\_a\_id) | n/a |
| <a name="output_private_subnet_b_id"></a> [private\_subnet\_b\_id](#output\_private\_subnet\_b\_id) | n/a |
| <a name="output_public_subnet_a_id"></a> [public\_subnet\_a\_id](#output\_public\_subnet\_a\_id) | n/a |
| <a name="output_public_subnet_b_id"></a> [public\_subnet\_b\_id](#output\_public\_subnet\_b\_id) | n/a |
| <a name="output_vpc_id"></a> [vpc\_id](#output\_vpc\_id) | n/a |
<!-- END_TF_DOCS -->