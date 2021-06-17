# Baccus_Udacity_Cloud_devOps_proj2

BaccusFinalProject2.yml is the template-body YAML script.

Baccus-params.json is the parameter file with parameter definitions.

The entire YAML template will execute and build the whole network infrastructure including 2 Load Balancers, VPC, 2 Public subnets, 2 Private subnets, associate all of the relevant subnets with route tables, and then build the WebAppGroup, WebAppLaunch Config, and tie to the Load balancers.  Finally the Outputs will report back the health checks of the Load balancers.

The webpage should show the Udagram build site that gets copied from the S3 bucket.
