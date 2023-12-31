#### Application Overview
The application architecture uses AWS Lambda, Amazon API Gateway, Amazon DynamoDB, Amazon Cognito, and AWS Amplify Console. Amplify Console provides continuous deployment and hosting of the static web resources including HTML, CSS, JavaScript, and image files which are loaded in the user's browser. JavaScript executed in the browser sends and receives data from a public backend API built using Lambda and API Gateway. Amazon Cognito provides user management and authentication functions to secure the backend API. Finally, DynamoDB provides a persistence layer where data can be stored by the API's Lambda function.
#### Application Architecture Diagram
![image](https://github.com/hhoang91/wildrydes-site/assets/102393576/9de5cd74-9375-4763-b563-0055f48d0b41)
#### Website Link
Site link: https://main.dsukhgbsdywfn.amplifyapp.com/
#### Known Issue
The website is currently unable to send verification codes to any email addresses except for those verified within the domain. This limitation arises because AWS SES places new accounts' SES service in sandbox mode, which grants limited access to certain features until Amazon approves the account after a request is sent. Which explained why I was able to demonstrated all the website’s features with my email. Further information can be found here: https://docs.aws.amazon.com/ses/latest/dg/request-production-access.html.
