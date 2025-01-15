Serverless Message Board Application

My Serverless Message Board Application is a fully serverless web application designed to allow users to submit messages via a web form. The messages are stored in an Amazon DynamoDB table and can be displayed on the web page upon refreshing the content. This implementation leverages several AWS services, including Amazon S3 for static web hosting, AWS Lambda for serverless compute, Amazon API Gateway for managing API requests, and Amazon DynamoDB for data storage.

http://my-message-board-rg317.s3-website-us-east-1.amazonaws.com/


Project Completion Steps
Set Up AWS Services: Initiate the necessary AWS services including S3, Lambda, API Gateway, and DynamoDB.

Create an S3 Bucket: Configure an Amazon S3 bucket to host the static website. Upload the index.html file to this bucket and set the appropriate bucket policy for public access.

Deploy DynamoDB Table: Create a DynamoDB table based on the specifications found in the Lambda function code. Identify the table name and partition key and set the read/write capacity as needed.

Implement AWS Lambda Function: Deploy the provided lambda_code.py as an AWS Lambda function. This function will handle the logic for storing messages in DynamoDB and retrieving them.

Set Up API Gateway: Create a REST API using Amazon API Gateway. Configure the API to proxy requests to the Lambda function for both posting new messages and retrieving existing messages. Ensure that the resource path and HTTP methods are correctly defined as per the index.html code.

Configure CORS: Set up Cross-Origin Resource Sharing (CORS) settings in the API Gateway to allow the S3 hosted website to interact with the API without restrictions.

Permissions: Ensure that the appropriate IAM roles and policies are assigned to the Lambda function, allowing it to read and write to DynamoDB.

Testing: After deployment, test the application by submitting messages through the form and verifying that they are stored in DynamoDB and displayed correctly on the webpage.

Cloud Skills Required
To successfully complete this project, the following cloud skills are essential:

AWS Core Services: Knowledge of AWS services like S3, Lambda, API Gateway, and DynamoDB.
Serverless Architecture: Understanding of serverless application design principles.
IAM and Permissions Management: Familiarity with AWS Identity and Access Management (IAM) to set permissions for accessing resources securely.
API Development: Proficiency in designing and deploying RESTful APIs, including handling CORS configurations.
Frontend Development: Basic skills in HTML and JavaScript to build the user interface.
Success Validation

To validate successful deployment, ensure that you can:

Post messages to the DynamoDB table through the S3 website form.
Retrieve and display the messages on the webpage by refreshing the content.
With these steps and skills, you should be able to create a fully functional serverless message board application.
