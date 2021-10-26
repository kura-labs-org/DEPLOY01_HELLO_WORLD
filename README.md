# DEPLOY01_HELLO_WORLD

The 


Ssh into your EC2 using the directory the key is in or simply copy the path the key is and ssh into it. Mine would be ssh -i Aws-key-pair1.pem ec2-user@3.92.210.123 for deployment 1 or you just go into your downloads and copy the path to the aws key and ssh into  it. Ex ssh -i C:\Users\jpl28\Downloads\Aws-key-pair1.pem ec2-user@184.72.208.64
When I tried to do sudo systemctl daemon-reload I got Error: Package: jenkins-2.303.1-1.1.noarch (jenkins) Requires: daemonize
https://stackoverflow.com/questions/68806741/how-to-fix-yum-update-of-jenkins has the solution to fix it.
sudo amazon-linux-extras install epel -y
sudo yum update -y
sudo yum install jenkins java-1.8.0-openjdk-devel -y
After I typed systemctl daemon-reload I got this error : Failed to execute operation: The name org.freedesktop.PolicyKit1 was not provided by any .service files
I typed in sudo in front of  systemctl daemon-reload and I didn’t get an error so I believed it worked. I then stated jenkins with sudo systemctl start jenkins
I checked the status of jenkins with sudo systemctl status jenkins
It worked and was up and running. I checked by accessing my IPv4 address with port 8080. Ex 3.92.210.123:8080
Then I cat (cat is a linux command that reads the file and reads you what’s inside the file ) sudo cat /var/lib/jenkins/secrets/initAdminPassword
I get the key inside and I paste it in the form and then proceed to set up my password and account
I install git in my EC2 with sudo yum install git -y
Use the git version command to verify that its installed in the EC2 instance
Go into Jenkins, click create a new item and give it a name Jenkins-webhook


![Screenshot (246)](https://user-images.githubusercontent.com/16675605/138932517-dc24b6e5-73db-4b12-b7e5-d6cea63af803.png)

![Screenshot (247)](https://user-images.githubusercontent.com/16675605/138932611-3739f7e3-d418-40c0-9d61-b2031cf2bbd1.png)

