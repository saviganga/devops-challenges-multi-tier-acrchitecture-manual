# devops-challenges-multi-tier-acrchitecture-manual


This project manually deploys a Multi-tier architecture stack on Virtual Machines runnung locally using Vagrant

# STACk
The stack for this project consists of:
- mysql: for the database 
- memcached: to serve as the database cache - this is used to improve the performance of the application by caching db queries
- rabbitMQ: to serve as the message broker
- nginx: to serve as the application load balancer
- tomcat: to serve as the web application server
- java: to serve as the runtime environment for the application

# STEPS
1. setup the backend infrastructure - database, cache, message broker
    - setup and install mysql service on the VM designated as the database server
    - clone java application code, and migrate the database schema
    - setup and install memcached service on the VM designated as the cache server
    - setup and install rabbitMQ service on the M designated as the message broker server