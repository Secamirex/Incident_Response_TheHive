# TheHive Incident Response 
![image](https://github.com/user-attachments/assets/f0ccd7e4-a9c9-4016-9855-f2f3daa38cd4)

<h2> Lab Objective:  
  To install TheHive, Cortex and MISP paltforms using docker compose and yml config file. </h2>

Note : This installation will be carried out via Docker compose method.
Docker compose allow us to run multiple containers at once  using YML file in which we set up each service variables, ports, image etc.

<strong> TheHive: </strong>
Is an open source and free Security Incident Response Platform designed to make life easier for SOCs, CSIRTs, CERTs and any information security practitioner dealing with security incidents that need to be investigated and acted upon swiftly.
It is the perfect companion to MISP. You can synchronize it with one or multiple MISP instances to start investigations out of MISP events

<strong> Cortex: </strong> 
created by TheHive team, analyses Observables, such as IP and email addresses, URLs, domain names, files or hashes, can be analysed one by one or in bulk mode using a Web interface.
 

<strong> MISP: </strong>
is an open source threat intelligence and sharing platform helps correlate, share and analyse information about targeted attacks 

<strong> Configuration Steps </strong>
 
1. Download the latest  docker compose YML file for the lab from the GitHub  link below
    
[thehive-cortex-misp-docker-compose-lab11update/docker-compose.yml at main · ls111-cybersec/thehive-cortex-misp-docker-compose-lab11update · GitHub](https://github.com/ls111-cybersec/thehive-cortex-misp-docker-compose-lab11update/blob/main/docker-compose.yml) 
	
3. Install Docker on the Ubuntu Server (If not installed) . Refer to  this link for more details.

https://docs.docker.com/engine/install/ubuntu/

4. Create a directory on Ubuntu and copy the YML file in there.
5. Run <strong>  'sudo docker-compose  up' </strong> command 

![image](https://github.com/user-attachments/assets/b20a47b6-d21e-4c38-8013-cf97ddf748bb)

6. Instructions on how to install docker-compose on Ubuntu  can be found on the link below.
   
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-20-04

![image](https://github.com/user-attachments/assets/0b999b4c-708d-4d0f-a2d2-85fbd72d1bd4)

7. Once installation completes, check the docker processes. The following  services should be up and running as shown below.

* Misp
* Cortex
* Cassandra
* Elasticsearch
* Minio
* Mysql-server
* redis


![image](https://github.com/user-attachments/assets/05a69c80-1d7c-4edb-bb35-37708a66a9b0)

<h2>TheHive Web UI</h2>

![image](https://github.com/user-attachments/assets/ee32f2aa-0ca4-491d-93eb-13b902e1dcde)

<h2>Cortex Web UI</h2>

Note: Cortex database needs to be updated before performing initial configurations. 

![image](https://github.com/user-attachments/assets/5a0573ea-9fb6-4958-918b-a95f65509279)


<h2>MISP Web UI</h2>

![image](https://github.com/user-attachments/assets/503b56ec-d09f-4a03-a1c1-27fcf98ce19c)


