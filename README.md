<h1>Deploying Infra as Code in AWS with Serverless Framework</h1>
<h2>Objective</h2>
Deploy services to Create, Read, Update and Delete (CRUD) items in a DynamoDB table, through Node.js API endpoints, over AWS Lambda functions, using the Serverless Framework.
<h2>About Serverless Framework</h2>
"The Serverless Framework pioneered serverless architecture on AWS, a transformative approach to building applications on cloud infrastructure that auto-scales, incurs no charges when idle, and typically demands minimal maintenance. Today, it continues to be the leading developer tool for deploying serverless architectures." <br>
"The Serverless Framework helps you develop and deploy AWS Lambda functions, along with the AWS infrastructure resources they require. It's a CLI that offers structure, automation and best practices out-of-the-box, allowing you to focus on building sophisticated, event-driven, serverless architectures, comprised of Functions and Events."<br>
<h3>Key concepts of Serverless Framework</h3>
1. <b>Functions</b>: The code of a serverless application is deployed and executed in AWS Lambda functions.<br>
2. <b>Events</b>: Functions are triggered by events, that come from other AWS resources, for example, an HTTP request on an API Gateway.<br>
3. <b>Resources</b>: Resources are AWS infrastructure components used by the functions, such as a DynamoDB table, for example.<br>
4. <b>Services</b>: A service is an unit of organization. A service is configured via a file called <u>serverless.yml</u>, where you define your functions, events and resources.<br>

See: [Serverless documentation](https://www.serverless.com/framework/docs)