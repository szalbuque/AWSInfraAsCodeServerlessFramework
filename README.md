<h1><b>Deploying Infra as Code in AWS with Serverless Framework</b></h1>
<h2><b>Objective</b></h2>
Deploy services to Create, Read, Update and Delete (CRUD) items in a DynamoDB table, through Node.js API endpoints, over AWS Lambda functions, using the Serverless Framework.
<h2><b>About Serverless Framework</b></h2>
"The Serverless Framework pioneered serverless architecture on AWS, a transformative approach to building applications on cloud infrastructure that auto-scales, incurs no charges when idle, and typically demands minimal maintenance. Today, it continues to be the leading developer tool for deploying serverless architectures." <br>
"The Serverless Framework helps you develop and deploy AWS Lambda functions, along with the AWS infrastructure resources they require. It's a CLI that offers structure, automation and best practices out-of-the-box, allowing you to focus on building sophisticated, event-driven, serverless architectures, comprised of Functions and Events."<br>

<h3><b>Key concepts of Serverless Framework</b></h3>

1. <b>Functions</b>: The code of a serverless application is deployed and executed in AWS Lambda functions.<br>
2. <b>Events</b>: Functions are triggered by events, that come from other AWS resources, for example, an HTTP request on an API Gateway.<br>
3. <b>Resources</b>: Resources are AWS infrastructure components used by the functions, such as a DynamoDB table, for example.<br>
4. <b>Services</b>: A service is an unit of organization. A service is configured via a file called <u>serverless.yml</u>, where you define your functions, events and resources.<br>

<a href="https://www.serverless.com/framework/docs" target="_blank">See Serverless Framework Documentation</a>

<h2><b>Requirements</b></h2>

<h3><b>AWS account</b></h3>

It´s necessary to have an account, created in the AWS IAM with programmatic access, with the right permissions to access the resources used in the project. For this exercise, I´ll use an account with administrative access, but this is not the best practice.

<h3><b>Node.js installed</b></h3>

<a href="https://nodejs.org/en" target="_blank">See Node.js Documentation</a>

<h3><b>Serverless framework installed</b></h3>

> npm i -g serverless

<h3><b>The code</b></h3>

The code was developed by Cassiano Peres, and it´s available at: <a href="https://github.com/cassianobrexbit/dio-live-serverless-2907/tree/master/src" target="_blank">GitHub Repository</a>

<h3><b>The serverless.yml file</b></h3>

The serverless.yml file contains all the specifications necessary to create the AWS resources and deploy the Lambda Functions.

<h4><b>Specify the resources (in this case, the DynamoDB table):</b></h4>

![](images/resources.png)

<h4><b>Give access over DynamoDB for Lambda functions:</b></h4>

![](images/iamacess.png)

<h4><b>For each function, specify the name, the handler, the path and the method associated:</b></h4>

![](images/functions.png)


<h3><b>Postman installed</b></h3>

To test the API, install Postman. See:   <a href="https://www.postman.com/downloads/" target="_blank">Postman download</a>

