# Parking_Lot app

This project contains source code and supporting files for a serverless application that you can deploy with the SAM CLI. It includes the following files and folders.

- parking_lot - Code for the application's Lambda function.
- template.yaml - A template that defines the application's AWS resources.

The application uses several AWS resources, including Lambda functions and an API Gateway API. 

## Deploy the sample application

The Serverless Application Model Command Line Interface (SAM CLI) is an extension of the AWS CLI that adds functionality for building and testing Lambda applications. 
To use the SAM CLI, you need the following tools.

* AWS CLI -  [Install the AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
* SAM CLI - [Install the SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
* [Python 3 installed](https://www.python.org/downloads/)

To build and deploy your application for the first time, run the following in your shell:

```bash
sam build 
sam deploy 
```

## Api endPoints
At the end of the deployment two API test stage endpoints will be shown, already with query parameters examples for your convenience:<br/>
1 - HttpApiEntryGateway:  the entry POST call <br/>
2 - HttpApiExitGateway: the exit POST call <br/>
Just copy and paste them when creating a POST request using a API testing application 

###Enjoy!
## Cleanup

To delete the sample application that you created, use the AWS CLI.
```bash
aws cloudformation delete-stack --stack-name parkingLot-app
```
