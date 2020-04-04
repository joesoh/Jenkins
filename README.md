# Jenkins
This Repo outline the procedure in upgrading Jenkins

Obtain Jenkins war file from 
https://updates.jenkins-ci.org/download/war/

Command wget https://updates.jenkins-ci.org/download/war/2.150.3/jenkins.war

Confirm locatio of running Jenkins
ps -eaf | grep java

 
Remove symlink
rm jenkins.war
 
Create symlink and link it to new war file
ln -s jenkins-2.150.3.war jenkins.war
 
Restart Jenkins

systemctl restart jenkins
 
Check Log
tail -f /var/log/jenkins/jenkins.log

