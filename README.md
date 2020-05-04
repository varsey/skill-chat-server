# chat-server
Websocket chat server

Server part of simple adnroid cryptochat:
https://github.com/varsey/simple-android-cryptochat

Create virtual machine open: ext (Ingress) IP: 0.0.0.0/0  TCP port 8881

#prereq
sudo su
apt-get update
apt-get install openjdk-8-jdk maven -y

#clone server proj
git clone https://github.com/varsey/skill-chat-server

#unpack it
tar -xzf ./chat-server.tar.gz

#run inside of unpacked folder:
mvn clean install
mvn exec:java
