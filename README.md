# AppleBite
This repository is for the Edureka DevOps certification project


# Steps For executing the solution:

CICD Setup:


- Use the Master server for Jenkins, Ansible, Git etc.

- created a Master server on Ubuntu(22.04) and installed jenkins, Ansible, Git.

Jenkins: 

![image](https://user-images.githubusercontent.com/125067454/232808173-703d9a37-a706-4a41-b8d4-e45fde7d4513.png)


Ansible :

![image](https://user-images.githubusercontent.com/125067454/232808540-c7763930-97ab-425c-84ff-8e8251e3e0a5.png)


Git :

![image](https://user-images.githubusercontent.com/125067454/232808867-0c8c49ff-78ad-4b4f-a946-99c1121e8030.png)


- User another server Ubuntu(22.04) for Jenkins Slave Node


![image](https://user-images.githubusercontent.com/125067454/232810638-fc85ab71-ad5d-43da-86d2-c2da507e1f51.png)




- Add Build Pipeline Plugin and Post -build task plugin to Jenkins on the Master server

Install Python, Open ssh-server and git on the slave node manually


Python :

![image](https://user-images.githubusercontent.com/125067454/232811577-0e493ebc-d59d-4b9f-9035-7f820dd119c9.png)


Openssh-server :


![image](https://user-images.githubusercontent.com/125067454/232811888-af13a3b2-2809-4726-9f67-7bf95743f869.png)




- Use the image devopsedu/webapp and add PHP website to it using a Dockerfile


![image](https://user-images.githubusercontent.com/125067454/232816464-fd187ab8-4a03-41e8-b4eb-5ef0851d057c.png)




![image](https://user-images.githubusercontent.com/125067454/232816653-e996deea-9880-4ee6-ba50-9942df084081.png)










- Push the PHP website and Dockerfile to a git repository

- Then Created CI/CD pipeline for automation:

Job1- Install Puppet Agent on Slave


![image](https://user-images.githubusercontent.com/125067454/232814393-e97a8e76-6c81-4466-8d90-805c89f4fa4a.png)



Job2 : Sign the Puppet certificate


Job3 : Install Docker on the Jenkins Slave server









![image](https://user-images.githubusercontent.com/125067454/232806310-713bcc2c-9b96-4b21-b19e-bcb0e6418906.png)




![image](https://user-images.githubusercontent.com/125067454/232809707-097ac7a7-12f5-4264-943b-87d67cb14388.png)
