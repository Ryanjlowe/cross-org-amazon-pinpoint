# Amazon Pinpoint Cross Org Project Setup

Includes the infrastructure, policies, and example code needed to implement sharding Amazon Pinpoint projects across multiple AWS Accounts inside of an AWS Organization.  Useful for scenarios where more than 100 Pinpoint Projects are needed.

## Architecture Diagram

![Arch](arch.png)

*DynamoDB and Lambda with STS logic not included

## Files
* [PrimaryAccount.yaml](PrimaryAccount.yaml) - Used to set up assets in the Primary Account
* [SubAccount.yaml](SubAccount.yaml) - Used to set up assets in each Sub Account
* [PinpointProject.yaml](PinpointProject.yaml) - Used to set up each Pinpoint Project in sub accounts
