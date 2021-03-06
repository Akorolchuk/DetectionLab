# DetectionLab Terraform

### Method 1 - Building the VMs locally and exporting them to AWS as AMIs
One method for spinning up DetectionLab in AWS is to begin by using Virtualbox or VMware to build DetectionLab locally. You can then use AWS's VM import capabilities to create AMIs based off of the virtual machines. Once that process is complete, the infrastructure can easily be spun up using a Terraform configuration file.

This method has the benefit of allowing users to customize the VMs before importing them to AWS.

The instructions for deploying DetectionLab in AWS via this method are available here: [Build Your Own AMIs README](./VM_to_AMIs.md)


### Method 2 - Pre-built AMIs
As of March 2019, I am now sharing pre-built AMIs on the Amazon Marketplace. The code inside of main.tf uses Terraform data sources to determine the correct AMI ID and will use the pre-built AMIs by default.

Using this method, it should be possible to bring DetectionLab online in under 15 minutes.

The instructions for deploying DetectionLab in AWS using the pre-built AMIs are available here: [Pre-Built AMIs README](./Pre-Built_AMIs.md)
