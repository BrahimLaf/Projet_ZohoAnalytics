# Projet Final Docker/BI : Zoho Analytics On-Premise

## Projet Zoho Analytics On-premise

### 1. Objectif of project 

The objective of mon project is to use a Busness intelligence solution Zoho Analytics On-Promise via Docker to do the containerization.

Zoho Analytics is a self-service BI and data analytics software that lets you analyze your data, create stunning data visualizations, and discover hidden insights in minutes

### 2. Explication du docker-compose.yml

### 3. Architecture

This image represents my architecture that I used for the realization of mon project. Indeed, I used Zoho Analytics On-Premose, Postgres and PgAdmin linked via a docker-compose.yml file on a microsoft azure virtual machine. I then, using the Zoho Analytics On-premise, visualized the data from I database in Postgres.

### 4. Steps to deploy

###### Step 1. 
###### Step 2. Check the containers that are running using the following command: docker ps

###### Step 3. Execute an interactive bash shell on the downloaded container using the following command: sudo docker exec -it projet_zohoanalytics-Web-1 bash

###### Step 4. Before starting the application, switch to the Zoho/Analytics/bin repository.

###### Step 5. Start Zoho Analytics On-Premise using the command: nohup sh app_ctl.sh run &. 

###### Step 6. Once the application has started, you can access the application from a web-browser using the following URL https://serverIPaddress:8443.

###### Step 7. Use the following credentials in the screen that appears to login to Zoho Analytics On-Premise the default password upon login is :
  ###### Username: admin
  ###### Password: admin

###### Step 8. Use the command disown to remove jobs from the job table of the parent shell


###### Step 9. To stop the application, use the following command: sh app_ctl.sh shutdown




