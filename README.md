sudo yum update
sudo yum install java
java --version
wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.58/bin/apache-tomcat-9.0.58.tar.gz
tar xfvz apache-tomcat-9.0.58.tar.gz
cd apache-tomcat-9.0.58
cd webapps/manager/META-INF/
ls
vi <ur filename>
comment ip address retriction and save and exit the file(press esc & :wq!)
./startup.sh
Use public Ipv4 address of ur ec2 machine and hit on the browser with <Ipaddress>:8080
if you got an error like site cant be reached follow below steps
1. enter into security groups of your machine
2. edit inbound rules
3. add all traffic and source as anywhere and save your configuration


<role rolename="manager-gui"/>
<user username="admin" password="password" roles="manager-gui"/>

https://github.com/anilkumar23/AWS-Batch-1
