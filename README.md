# **JAVA SPRINGBOOT PROJECT**
---
## Flow of Execution
- AWS cloud Infrastructure was deployed in this project.
* VPC setup was done to have control over our network enviroment and provide security measures.
* Continous Integration Setup using jenkins and sonarqube( to perform code analysis for vulnerability test).
* Dockerhub account used to containerize our project.
* Stored Dockerhub credentials in jenkins.
* Stored Docker Engine in jenkins.
* Installed the following pluggins in jenkins (Docker-pipeline,Docker and pipeline utility ).
* Created kubernetes cluster with kops. 
* Installed helm in kops Server.
* Created helm charts which was used to package and deploy our entire stack.
* Added kops server as a jenkins slave.
* Updated the following in our git repository (helm chart,dockerfile,jenkins pipeline code).
*  Created jenkins job for pipeline.
*  Run and test the job.
## **Analysis of Our Github Repository(cicd-kube-spring .main branch)**
---
[ github link](https://github.com/easyboss1/cicd-kube-spring.git)
- helm directory consist of a template directory in it which contains all our secret,service and deployment files for postgres database,RabbitMQ,memcached,Springboot app . 
- src directory contains the source files needed to the source files needed for our springboot app deployment. 
- Dockerfile which consist of a text-based script instructions used to build our Springboot app container image.
- jenkinsfile consist of our pipeline code.  
- pom.xml file contains information for maven to build the project.
