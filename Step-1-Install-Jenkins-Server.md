![Jenkins](https://github.com/silviob99/Project-3-Deployment-Automation-with-Continuous-Integration-Introduction-to-Jenkins/assets/107585020/855c901b-0301-4d3a-9892-f6aefb04cf6d)

## Project-3-Deployment-Automation-with-Continuous-Integration-Introduction-to-Jenkins

### Install Jenkins Server 
1. Create an AWS EC2 server based on Ubuntu Server 20.04 LTS and name it "Jenkins"
2. Install JDK (since Jenkins is Java based application)

```
sudo apt update
sudo apt install default-jdk-headless
```

3. Install Jenkins

```
wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \
    /etc/apt/sources.list.d/jenkins.list'
sudo apt update
sudo apt-get install jenkins
```

Make sure Jenkins is up and running  

```sudo systemctl status jenkins```  
4. By default Jenkins server uses TCP port 8080 - open it by a new Inbound rule in your EC2   
