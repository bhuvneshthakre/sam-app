1.Install and configure AWS CLI and SAM CLI on your local machine.

2. Create a new directory for your project and navigate to it in your terminal.

3. Run the following command to create a new SAM application:
sam init—runtime python3.8—name helloworld-app-template hello-world

4. This will create a basic SAM application structure in the current directory
with a sample
app.py file.
5. edit the contents of app.py with the following code:
def lambda_handler(event, context):
return {
'statusCode': 200,
'body': 'Hello, World!'
}
6. Deploy the application using the following command:
sam build
&&
sam deploy-guided

7.open cloud formation and after some time the app will be deployed

8.open the aws service lambda and
The lambda function is created & the api gateway is triggered the url is as
follow

9. https://rrz3qrwwu1.execute-api.us-east-1.amazonaws.com/Prod/hello
