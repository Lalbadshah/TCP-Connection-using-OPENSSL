# TCP-Connection-using-OPENSSL
Server and Client programs using the openssl libraries to establish a tcp connection
# Generating a certificate
Execute this command:
openssl req -x509 -nodes -days 365 -newkey rsa:1024 -keyout mycert.pem -out mycert.pem
#To run the Server
Compile : gcc -Wall -o ssl-server SSL-Server.c -L/usr/lib -lssl -lcrypto
Run : sudo ./ssl-server <portnum> 

#To run the Client 
Compile : gcc -Wall -o ssl-client SSL-Client.c -L/usr/lib -lssl -lcrypto
Run : ./ssl-client <hostname> <portnum> 



