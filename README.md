# nodejs-sendmail
A NodeJS application to send mail using Amazon SES

## How to use

- Configure your Amazon AWS credentials on your environment ([Tutorial here](https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/loading-node-credentials-shared.html));
- Download the project as **.zip**;
- Enter into project directory and run **npm install**;
- Run **npm app.js**;

- Try it using **Postman** or **cURL**, e.g.: curl --data "fromaddress=<FROM_ADDRESS>&toaddresses=<TO_ADDRESSES>&subject=Test mail&text=This is a test mail" http://localhost:3000/mail/send

## Parameters per endpoint
### mail/send
- fromaddress: Email address from where the e-mail will be sent;
- toaddresses: Email addresses that will receive the mail message;
- subject: Subject of the mail;
- text: Message of the mail;
- replytoaddress (optional): Email address to where the receiver will reply.