
1. Review the template 1.webserver.template
2. Login to AWS account and go to CloudFormation
3. Create stack using the template Create stack with the following parameters:

* Stack name: cfinit-test
* Instance Type: t1.micro
* KeyName: Your keyname, you should create one if you do not have one
* SSLLocation: 0.0.0.0/0

4. Review outputs and confirm everything is fine and access the URL in the output

5. Does it work? If not, fix the error and update the stack ( corrected solution is in 2.webserver.template file)


To debug the error, SSH in to the server, and review the contents of the file using:

cat /var/log/cloud-init-output.log 

Look at the bottom to see any errors reported by cfn-helper and fix those errors. 

6. Keep trying until it all works
