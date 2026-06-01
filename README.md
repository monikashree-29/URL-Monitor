The URL Monitoring & Alert System is a serverless cloud-based solution designed to continuously monitor the availability and health of a website and notify administrators when downtime is detected. 
The project leverages multiple AWS services to provide automated monitoring, alerting, and logging capabilities.
The system uses Amazon EventBridge to trigger a monitoring process at scheduled intervals (for example, every 5 minutes). 
EventBridge invokes an AWS Lambda function, which acts as the core processing component. 
The Lambda function sends an HTTP request to the target website URL and checks whether the website is reachable and responding correctly.
If the website is unavailable or returns an error, the Lambda function publishes an alert message to an Amazon SNS (Simple Notification Service) topic.
SNS then delivers real-time notifications to subscribed email addresses, enabling administrators to take immediate action.
The project uses AWS IAM roles and policies to securely grant the Lambda function permission to access SNS and other required AWS resources.
Additionally, Amazon CloudWatch Logs automatically records Lambda execution details, request outcomes, and error messages, helping with monitoring, troubleshooting, and auditing.
This serverless architecture eliminates the need for dedicated servers, reduces operational overhead, and scales automatically. 
The project demonstrates practical knowledge of AWS monitoring, automation, event-driven architecture, security management, and cloud-native application development.
