# nodejs-express-on-aws-ec2
This my 1st nodejs app deployment using codedeploy on aws ec2

EC2 user script to install codedeploy agent:- 
--------------------------------------------------
#!/bin/bash
sudo yum -y update
sudo yum -y install ruby
sudo yum -y install wget
cd /home/ec2-user
wget https://aws-codedeploy-us-east-1.s3.amazonaws.com/latest/install
sudo chmod +x ./install
sudo ./install auto
------------------------------------------------------
