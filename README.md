**Name:** Bhavdip Akabari  
**Company:** Codtech It Solutions  
**ID:** CT12DS2309 
**Domain:** Cloud Computing Intern  
**Duration:** Aug To Oct 2024  
**Mentor:** Muzammil Ahmed  

## Overview of the Project

### Project: BUILDING A SERVERLESS APPLICATION WITH AWS LAMBDA

### Objective: 
This project implements a simple REST API endpoint using AWS Lambda and API Gateway. The goal is to explore serverless computing and understand the basics of Lambda function deployments with HTTP API integration on AWS.

### Architecture:
- AWS Lambda: Function handles the core business logic and responds to API requests.
- API Gateway: Exposes the Lambda function as a REST API endpoint.
- IAM: Manages permissions for secure access and invocation.

### Prerequisites:
- AWS account (Sign up if you don't have one).
- Basic knowledge of serverless concepts and AWS Lambda.
- AWS CLI installed and configured (installation guide).

### Setup and Deployment: 
- **Step 1:Setup and Deployment**
  - git clone https://github.com/your-username/your-repo-name.git
  - cd your-repo-name
- **Step 2: Create the Lambda Function**
  - Go to AWS Console > Lambda.
  - Create a new function (e.g., HelloWorldFunction) and select Author from scratch.
  - Configure the function with the necessary execution role (e.g., AWSLambdaBasicExecutionRole).
  - Add your function code and test the function in the AWS Console.  
- **Step 3: Set Up API Gateway**
  - Open API Gateway in the AWS Console and create a REST API.
  - Configure Method (e.g., GET) for your endpoint, integrating it with the Lambda function.
  - Deploy the API to a stage (e.g., prod) to obtain the Invoke URL.
- **Step 4: Deploy the API**
  - Go to the Stages section in API Gateway.
  - Select your stage and copy the Invoke URL to test your endpoint.

- ![image](https://github.com/user-attachments/assets/77f1caea-571a-4e0f-8707-656f92ea1fae)
- ![image](https://github.com/user-attachments/assets/59ba5f5b-2c15-4b63-8d6d-910c5c5f147f)



### Usage:
  - 1.Invoke the Endpoint: Access the API endpoint using the Invoke URL provided after deployment.
    - curl -X GET https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello
  - 2.Expected Response:
    - {
       "message": "Hello, World!"
      }

### Technology Used: 
Python
API
AWS LAMBDA

### Troubleshooting:
- "Missing Authentication Token": Ensure the URL includes the stage name and resource path (e.g., /prod/hello).
- Lambda Permissions: Make sure API Gateway has permission to invoke the Lambda function. Run add-permission command if needed.

