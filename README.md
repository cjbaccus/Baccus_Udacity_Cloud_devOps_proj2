# Baccus_Udacity_Cloud_devOps_proj2

BaccusFinalProject2.yml is the template-body YAML script

Baccus-params.json is the JSON formatted parameter file.

Right now, I am having issue with creation of the ServerInstance due to error 
``` No default VPC for this user. GroupName is only supported for EC2-Classic and default VPC. (Service: AmazonEC2; Status Code: 400; Error Code: VPCIdNotSpecified; Request ID: 5ded1911-3269-4997-b2a9-24bc699ca55b; Proxy: null)```
I point to the VPC with !Ref VPC (I used that in InternetGatewayAttachment: resource, and had no issue) but for the server it is asking for a 'default' VPC...

I execute the script from Powershell with the following:
``` aws cloudformation create-stack --stack-name BaccusProj2 --template-body file://BaccusFinalProject2.yml --parameters file://Baccus-params.json --region=us-east-1 --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM" ```
