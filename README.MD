## Install Jenkins on aws linux machine 

Hi, I am Gustavo & today we will learn:

1. How to download and install Jenkins on aws ec2 linux
2. How to access Jenkins from browser
3. How to start and stop Jenkins
4. How to start Jenkins on different port
5. How to uninstall Jenkins

**Step 1** : Connect to your Linux machine

**Step 2** : Update Packages
   sudo yum update

**Step 3** : Check Java is installed. If not install java  
   java -version
   sudo yum install java-1.8.0

   To check and select one out of multiple java versions available
   sudo /usr/sbin/alternatives --config java

**Step 4** : Download latest Jenkins code package
   sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenk...

**Step 5** : Import a key file from Jenkins-CI to enable installation from the package
   sudo rpm --import http://pkg.jenkins-ci.org/redhat/jenk...

**Step 6** : Install Jenkins
   sudo yum install jenkins

**Step 7** : Start jenkins
   sudo service jenkins start

**Step 8** : Access Jenkins server using the public DNS of your ec2 on port 8080
 