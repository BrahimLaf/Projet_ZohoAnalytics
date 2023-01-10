# Projet Final Docker/BI : Zoho Analytics On-Premise

## Projet Zoho Analytics On-premise

### 1. Objectif of project 

The objective of mon project is to use a Busness intelligence solution Zoho Analytics On-Promise via Docker to do the containerization.

Zoho Analytics is a self-service BI and data analytics software that lets you analyze your data, create stunning data visualizations, and discover hidden insights in minutes

### 2. Explication du docker-compose.yml

### 3. Architecture

This image represents my architecture that I used for the realization of mon project. Indeed, I used Zoho Analytics On-Premose, Postgres and PgAdmin linked via a docker-compose.yml file on a microsoft azure virtual machine. I then, using the Zoho Analytics On-premise, visualized the data from I database in Postgres.

### 4. Steps to deploy

###### Step 1. Launch docker compose .yml: 
       Sudo docker-compose -f Docker-compose.yml up -d
![image](https://user-images.githubusercontent.com/115103788/211642843-8beb1ae3-e286-409a-9a91-0842d6c35936.png)

###### Step 2. Check the containers that are running using the following command: 
        docker ps
![image](https://user-images.githubusercontent.com/115103788/211643113-77462843-2cf4-4093-bc9f-19f48a152f9f.png)

###### Step 3. Execute an interactive bash shell on the downloaded container using the following command:
        sudo docker exec -it projet_zohoanalytics-Web-1 bash
![image](https://user-images.githubusercontent.com/115103788/211643178-a5d963bf-7538-45b1-8977-e8aecde4f5a6.png)

###### Step 4. Before starting the application, switch to the Zoho/Analytics/bin repository. cd Zoho/ cd Analytics/ cd bin/
![image](https://user-images.githubusercontent.com/115103788/211643408-5b998285-2e56-4614-8542-56d8c44ddba3.png)

###### Step 5. Start Zoho Analytics On-Premise using the command: 
        nohup sh app_ctl.sh run &
![image](https://user-images.githubusercontent.com/115103788/211643492-4e9416d5-355f-46aa-b39c-1a1cd4d7ddd9.png)

###### Step 6. Once the application has started, you can access the application from a web-browser using the following URL https://serverIPaddress:8443.
        https://serverIPaddress:8443
###### Step 7. Use the following credentials in the screen that appears to login to Zoho Analytics On-Premise the default password upon login is :
    Username: admin
    Password: admin
![image](https://user-images.githubusercontent.com/115103788/211643664-3d8e9beb-6af1-4348-a9b0-5c4a001b2357.png)


![image](https://user-images.githubusercontent.com/115103788/211643721-810b07e4-0ce3-4b18-97fd-a8a98ef4d31d.png)

###### Step 8. Use the command disown to remove jobs from the job table of the parent shell


###### Step 9. To stop the application, use the following command: sh app_ctl.sh shutdown




