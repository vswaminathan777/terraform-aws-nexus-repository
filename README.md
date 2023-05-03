## ****************This Terraform Module is not supported by Sonatype**************** 

# Terraform Module for High Availability Sonatype Nexus Repository Deployment in AWS

## Example Usage

```hcl
module "nexus-repository" {
  source  = "vswaminathan777/nexus-repository/aws"
  nexus-license-file-path= "./nexus.lic"
  region="us-west-2"
  azs_list=["us-west-2b", "us-west-2a"]  
  profile= "aws-nexus-profile"
}
```