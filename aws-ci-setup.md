Process setup for AWS-CI

1) Open Instances in the platform.
2) Connect to the instance.
3) use the following commands to install Jenkins :

   sudo wget -O /etc/yum.repos.d/jenkins.repo \
       https://pkg.jenkins.io/redhat-stable/jenkins.repo
   sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
   sudo dnf upgrade
   # Add required dependencies for the jenkins package
   sudo dnf install fontconfig java-17-openjdk
   sudo dnf install jenkins
   sudo systemctl daemon-reload

4) Run this commands in your instances.

5) To start the Jenkins use following commands :  

   sudo systemctl enable jenkins
   sudo systemctl start jenkins
   sudo systemctl status jenkins

6) Run the commands to start and check the status of the Jenkins in your instances.

7) Change the security inbound rules .Allow the code 8080 for accessing the Jenkins.
8) Use your ip-address following with 8080 to open Jenkins.
9) Create your own Jenkins profile using your details.

     Finally, We setup Jenkins in our instances.

                        THANK YOU.
