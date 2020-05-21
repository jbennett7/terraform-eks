# Terraform EKS
Leverage terraform-aws-modules project to build out an EKS cluster.

## Inputs
* __cidr\_block__ - CIDR block value to use when creating the VPC.
* __name\_prefix__ - Prefix name to use when nameing things.
* __az\_count__ - Number of availability zones to deploy the cluster to.
* __region__ - The region to deploy the cluster to.
* __role\_arn__ - AWS role to assume.

All `inputs` have sane defaults so no configuration required to test.

## To deploy
```
terraform init
terraform plan
terraform apply
```

## Other References
* Uses terraform modules from the `terraform-aws-modules` project for building out the VPC and the EKS cluster.
  * https://github.com/terraform-aws-modules/terraform-aws-vpc.git
  * https://github.com/terraform-aws-modules/terraform-aws-eks.git
