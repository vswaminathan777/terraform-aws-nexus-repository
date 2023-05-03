## ****************This Terraform Module is not supported by Sonatype**************** 

# Terraform Module for High Availability Sonatype Nexus Repository Deployment in AWS

## Example Usage

```hcl
module "nexus-repository" {
  source  = "vswaminathan777/nexus-repository/aws"
  nexus-license-file-path="./2022-sonatype-internal-rm-lc-fw-fwfa-10apps-10rm_users-1000lc_users-10fw_users.lic"
  region="eu-west-1"
  azs_list=["eu-west-1a", "eu-west-1b"]  
  profile="devnxrm" 
  nexus-repository-version="3.52.0"
  nexus-repository-instances-count=2
  instances_count={"desired_size"="2", "min_size"= "2", "max_size"= "2"}
}
```


