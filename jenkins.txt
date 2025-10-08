This is a file update
This is a new update
Installed Jenkins on an ubuntu machine from AWS 
Jenkins needs Java so use   apt install openjdk-21-jre-headless
Go to Jenkins website > based on the OS get the command to download jenkimng on your machine 
Get the key from jenkins website - sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key

Create a file for jenkins - echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null

update the package list - sudo apt update

Install Jenkins - sudo apt install Jenkins

Once installed, you can login to Jenkins GUI through the public ip of your machine on port 8080 - 15.223.64.99:8080
After restarting your machine, the public ip of your machine will change unless you have an elastic IP so reconnecting to jenkins make sure to use your new public ip address 

