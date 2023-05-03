##This Terraform Module is not currently supported by Sonatype 

# Terraform Module for High Availability Sonatype Nexus Repository Deployment in Amazon Web Services (AWS)

##Example Usage

module "nexus-repository" {
  source  = "vswaminathan777/nexus-repository/aws"
  version = "1.0.2"
  nexus-license-file-path= "./nexus.lic"
  region="us-west-2"
  azs_list=["us-west-2b", "us-west-2a"]  
  profile= "aws-nexus-profile"
}