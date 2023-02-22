# middleware-scripts1
#!/bin/bash
# discription sonarcube script
# Author: Nancy
# Date: 

# Start with user su - vagrant
sudo yum update -y

# Java 11 installation
# Update server

sudo yum update -y

# Java 11 installation
sudo yum install java-11-openjdk-devel -y

sudo yum install java-11-openjdk -y

# Download SonarQube latest versions on your serve

cd /opt

sudo yum install wget -y

sudo wget https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.3.0.51899.zip

# Extract packages/unzip

sudo unzip /opt/sonarqube-9.3.0.51899.zip

sudo unzip /opt/sonarqube-9.3.0.51899.zip

# Change ownership to the user and Switch to Linux binaries directory to start service

sudo chown -R vagrant:vagrant /opt/sonarqube-9.3.0.51899

cd /opt/sonarqube-x.x/bin/linux-x86-64 

 ./sonar.sh start

# Connect to the SonarQube server through the browser. It uses port 9000. 

sudo firewall-cmd --permanent --add-port=9000/tcp

sudo firewall-cmd --reload
 
