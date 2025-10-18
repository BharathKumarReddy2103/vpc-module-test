# vpc-module-test

This repository is dedicated to testing the [`terraform-aws-vpc`](https://github.com/BharathKumarReddy2103/terraform-aws-vpc) module. It provides a set of test configurations and examples to validate and demonstrate the usage of the VPC Terraform module.

## Overview

- **Purpose:** To test and showcase the features of the [`terraform-aws-vpc`](https://github.com/BharathKumarReddy2103/terraform-aws-vpc) Terraform module.
- **Module Under Test:** [`terraform-aws-vpc`](https://github.com/BharathKumarReddy2103/terraform-aws-vpc)
- **Usage:** Clone this repository and use the provided Terraform configurations to deploy and validate VPC resources using the referenced module.

## Getting Started

### Prerequisites

- [Terraform](https://www.terraform.io/downloads.html) installed
- AWS credentials configured (e.g., via `aws configure`)
- Access to clone both this repo and the [`terraform-aws-vpc`](https://github.com/BharathKumarReddy2103/terraform-aws-vpc) module

### How to Use

1. **Clone the Repositories**

   ```bash
   git clone https://github.com/BharathKumarReddy2103/vpc-module-test.git
   cd vpc-module-test
   ```

2. **Review Example Configuration**

   The main Terraform configuration will reference the `terraform-aws-vpc` module, typically like this:

   ```hcl
   module "vpc" {
     source = "github.com/BharathKumarReddy2103/terraform-aws-vpc"
     # ... add required variables and customization ...
   }
   ```

   Update variables in `main.tf`, `variables.tf`, or other configuration files as needed.

3. **Initialize and Apply**

   ```bash
   terraform init
   terraform plan
   terraform apply
   ```

   This will deploy the VPC infrastructure using the tested module.

## Folder Structure

- `main.tf`: Example configuration using the VPC module
- `variables.tf`: Input variables for the test setup
- `outputs.tf`: Output values after module deployment

## Referenced Module

For details about the VPC module, see:  
👉 [terraform-aws-vpc README](https://github.com/BharathKumarReddy2103/terraform-aws-vpc#readme)

## Customizing Tests

You can modify the example configurations to test different features and options provided by the module, such as:

- Custom CIDR blocks
- Public/private subnets
- NAT gateways
- Route tables
- Security groups

Refer to the [module documentation](https://github.com/BharathKumarReddy2103/terraform-aws-vpc#readme) for all available variables and outputs.

## Contributing

Feel free to open issues or PRs to add new test scenarios, improve documentation, or report problems with the test setups.

## License

This repository is licensed under the same terms as the [`terraform-aws-vpc`](https://github.com/BharathKumarReddy2103/terraform-aws-vpc) module. See the [LICENSE](LICENSE) file for details.

---
**Maintainer:** [BharathKumarReddy2103](https://github.com/BharathKumarReddy2103)