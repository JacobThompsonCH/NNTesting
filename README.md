#### Table of Contents
1. [Usage](#usage)
2. [Requirements](#requirements)
3. [Providers](#Providers)
4. [Inputs](#inputs)
5. [Outputs](#outputs)
## Usage
*various commands
<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | ~> 1.4.2 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 4.67.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 4.67.0 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_create_ec2_instance"></a> [create\_ec2\_instance](#module\_create\_ec2\_instance) | ./modules/ec2 | n/a |

## Resources

| Name | Type |
|------|------|
| [aws_eip.nelnet_addr](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_eip_association.eip_assoc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip_association) | resource |
| [aws_instance.nelnet_web](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |
| [aws_s3_bucket.example](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket_intelligent_tiering_configuration.example-filtered](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_intelligent_tiering_configuration) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_ami"></a> [ami](#input\_ami) | The default ami we will be using for our instances | `string` | `"ami-ekslinux"` | no |
| <a name="input_eip_name"></a> [eip\_name](#input\_eip\_name) | The name we will be assigning to our EIP | `string` | `"nelnet-dev-web-address"` | no |
| <a name="input_environment_name"></a> [environment\_name](#input\_environment\_name) | The default name of the environment we will be working with | `string` | `"dev"` | no |
| <a name="input_instance_name"></a> [instance\_name](#input\_instance\_name) | Value of the Name tag for the EC2 instance | `string` | `"nelnet-dev-web"` | no |
| <a name="input_instance_type"></a> [instance\_type](#input\_instance\_type) | The instance type our ec2's will be using | `string` | `"t2.micro"` | no |
| <a name="input_region"></a> [region](#input\_region) | The region we will be deploying resources within | `string` | `"us-east-1"` | no |
| <a name="input_volume_size"></a> [volume\_size](#input\_volume\_size) | The default size of our EBS volumes | `number` | `15` | no |
| <a name="input_volume_type"></a> [volume\_type](#input\_volume\_type) | The default volume type of our EBS volumes | `string` | `"gp3"` | no |

## Outputs

No outputs.
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
