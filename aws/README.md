
# Amazon Web Services

AWS


* https://searchaws.techtarget.com/tip/Manually-spin-up-an-EC2-server-instance-in-7-steps   
* https://medium.com/@nZenitram/spinning-up-an-ec2-instance-ef7e81044dc4
* https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html

Connecting to jupyter notebook

1. Create an account
*https://aws.amazon.com/console/
*Create free account
*Christine note: Haven't done this in awhile, hopefully it's straightforward


2. Open the Amazon EC2 console at https://console.aws.amazon.com/ec2/.
3. Launch instance > Launch instance
4. Select Deep Learning Base AMI (Ubuntu)
5. Choose instance type:
*Details on instance types here: https://aws.amazon.com/ec2/instance-types/
*Christine note: When I did this previously, I had to email a request for access to the GPU instances. Not sure if that's still the case
6. Review and launch
7. Select an existing key pair or create a new key pair
* Create a new key pair
* Download key pair
* Launch instances
8. View instances
* Find your instance id
9. Connect to instance
* Open terminal on your computer
*cd /Users/<your_username>/Downloads/
*chmod 0400 <your .pem filename>
*ssh -L localhost:8888:localhost:8888 -i <your .pem filename> ubuntu@<INSTANCEID> (remove the <>)
10. After connecting, in terminal type in 'jupyter notebook'. Should launch a jupyter notebook.
  
11. When you're done, make sure to stop the instance so you don't get charged. 
*Go to your AWS instance>Actions>Stop or Terminate instance

