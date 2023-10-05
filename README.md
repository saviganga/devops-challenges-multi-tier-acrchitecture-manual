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
    - install and setup mysql service on the VM designated as the database server
    - clone java application code, and migrate the database schema
    - install and setup memcached service on the VM designated as the cache server
    - install and setup rabbitMQ service on the VM designated as the message broker server
2. setup application server - tomcat
    - install and setup apache tomcat server on the VM designated as the application server
    - connect the application code to the backend servers and application server