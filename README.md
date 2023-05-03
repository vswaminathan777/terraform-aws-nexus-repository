##This Terraform Module is not currently supported by Sonatype**********

# Terraform Module for implementing the reference architecture for High Availability Sonatype Nexus Repository Deployment in Amazon Web Services (AWS)

##Example Usage

module "nexus-repository" {
  source  = "vswaminathan777/nexus-repository/aws"
  version = "1.0.1"
  nexus-license-file-path= <path to nexus License file>
  region="us-west-2"
  azs_list=["us-west-2b", "us-west-2a"]  
  profile= <aws-profile-name>
}