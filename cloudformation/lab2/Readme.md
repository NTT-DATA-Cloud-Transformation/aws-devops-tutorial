
1. Review the template for ec2 server
2. Login to AWS account  and go to CloudFormation
3. Create stack using the template Create stack with the following parameters:

* Stack name: demolive3
* Instance Type: m3.medium
* KeyName: Your keyname
* SSLLocation: 0.0.0.0/0
* Create IAM Resources: No

4. Review outputs and confirm everything is fine and access the URL in the output

5. Does it work? If not, fix the error and update the stack 
