# assessment
AWS architecture for a python based application running on EKS
=======================================================================================
The developer will use git in the local to push their code to github
==========================================================================================
Once in github repository we can either use github actions or gitLab to automate the CICD pipeline
====================================================================================================================================================================================================================
At the early stages of the code we have to implement a source code scanning to check for code smells, vulnerability and bugs. For a python based application we can use a flask8 for lint Test and a pytest for unit test and for a java based application we can use Sonarqube
========================================================================================================================================================================================================================
If the test is succesfull we can then proceed to build the script from the source code to obtain an executable package. In a GitLab environment we create a build stage and we can use a minimum OS ubuntu image to build our image.Requirements: MUST install all the necassary python packages 
===========================================================================================================================================================================================================================
The image can then be containerized with docker and pushed to a Dockerhub registry or ECR
=====================================================================================================================================================================================================================
A helm chart can then be created from the updated image and either deployed to EKS or can be stored in the artifactory for futur use.
