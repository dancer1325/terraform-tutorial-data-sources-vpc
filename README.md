# Learn Terraform data sources - VPC
Follow along [with this Hashicorp tutorial](https://developer.hashicorp.com/terraform/tutorials/configuration-language/data-sources).

## Goal
* Terraform data sources allows
  * importing data into your Terraform configuration

## Prerequisites
* Terraform [v1.2+](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) installed locally
* AWS account with [associated credentials](https://registry.terraform.io/providers/hashicorp/aws/latest/docs#authentication-and-configuration)
  * via
    * add in the 'provider' block
    * environment variables
      * 'AWS_ACCESS_KEY_ID'
      * 'AWS_SECRET_ACCESS_KEY'
      * 'AWS_REGION'
    * credential files
      * `aws config` & pass the 'AWS_ACCESS_KEY_ID' & 'AWS_SECRET_ACCESS_KEY'

## How to run?
* `terraform init`
* `terraform plan`
* `terraform apply`
  * `terraform appy -var aws_region=us-west-1`
    * pass another variable rather than default one
* `terraform destroy`

## Notes
* [aws_availability_zones](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/availability_zones)
* [terraform_remote_state](https://developer.hashicorp.com/terraform/language/state/remote-state-data)
* [aws_ami](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami)
* [terraform-aws-modules/vpc](https://registry.terraform.io/modules/terraform-aws-modules/vpc/aws/latest)
  * [input variables](https://github.com/terraform-aws-modules/terraform-aws-vpc?tab=readme-ov-file#inputs)
    * [azs](https://github.com/terraform-aws-modules/terraform-aws-vpc?tab=readme-ov-file#input_azs)