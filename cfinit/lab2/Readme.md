
1. Review the template 3.webserver.template
2. Login to AWS account and go to CloudFormation
3. Create stack using the template Create stack with the following parameters:

* Stack name: cfsignal-test
* Instance Type: t1.micro
* KeyName: Your keyname, you should create one if you do not have one
* SSLLocation: 0.0.0.0/0

4. Does it work? If it fails, find the error, and see how cfn-signal (or the lack of it) caused the stack creation to fail


