# Serverless Message Board Application

## Instructions

You are tasked with deploying a serverless application. The application allows the submission of messages through a form. The messages are then written as items in a DynamoDB table. The messages can then be displayed by clicking the refresh button on the form.

The application should include an Amazon S3 static website for the webform, an Amazon API Gateway REST API, an AWS Lambda function, and an Amazon DynamoDB table.

You must piece the application together with minimal details. The following is provided:
- AWS Lambda function code in the `lambda_code.py` file.
- Website HTML/JavaScript code in the `index.html` file.

## Tips

- The database name and partition key can be identified in the Lambda function code.
- The resource path required in the API can be identified in the index.html code.
- The API methods can also be identified in the index.html code.
- The API should proxy the request to Lambda for both methods.
- You will need to ensure correct permissions and cross-origin resource sharing settings.

The ultimate resource is resourcefulness! Use whatever tools and research you need to to assist with this task.

## Success Validation

To prove you have successfully deployed the application you should be able to post messages to the database using the S3 website form and then retrieve and display the messages on the webpage.
