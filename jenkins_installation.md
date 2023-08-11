Steps to install Jenkins on an Ubuntu machine. 

1. sudo apt-get update
2. sudo apt install openjdk-11-jre
3. java -version
4. curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee   /usr/share/keyrings/jenkins-keyring.asc > /dev/null
5. echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]   https://pkg.jenkins.io/debian-stable binary/ | sudo tee   /etc/apt/sources.list.d/jenkins.list > /dev/null
6. sudo apt-get update
7. sudo apt-get install jenkins
8. sudo systemctl enable jenkins
9. sudo systemctl start jenkins
10.sudo systemctl status jenkins

NOTE:
Make sure that port 8080 is open and accessible from internet. 
You can access your Jenkins instance at http://<serverpublicIP>:8080. It will ask you to unlock Jenkins: go to this file location /var/lib/jenkins/secrets/initialAdminPassword and copy the password to unlock your instance.