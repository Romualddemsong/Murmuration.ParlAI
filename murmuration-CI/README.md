setup GitLab environment and prepare the runners
#######################################################################################################################
use a build server to run prepare all the required packages for the python environment
install python3 to prepare the environment
## python3.8 -m venv venv
#########################################################################################################################
upgrade pip, setuptools and wheel packages within the python virtual envirornemnt with the command
## venv/bin/pip install --upgrade pip setuptools wheel
########################################################################################################################
configure the repository package list with the command
## apt-get update
######################################################################################################################
## Use the apt-get curl -y command to install the curl package
download the scipy package from github repository
## curl -OL https://github.com/scipy/scipy/archive/refs/tags/v1.12.0.tar.gz 
## unzip with tar -xvf v1.12.0.tar.gz 
## from the unzipped file cd into scipy and increase to permissions for the dev.py
## cd scipy-1.12.0
## chmod +x dev.py
## install click and doit packages with the respective command
## pip install click
## pip install doit
##  install parlAI with the *pip install parlai*
## run the devoleper test script to test the code and create and output file to store the artifacts



#####   TEST SUCCESSFULLY COMPLETED

#################################################################################################################


#### BUILD STAGE START###########################################################################################
use the latest docker image form the Dockerhub and containerize to artifact outputed from the test stage. We need to authenticate to the dockerhub account to be able to run the built script


############  QUESTION #############################################################################################
1) Where is the artifact from thr test stage stored



#########    Challenges faced#########################################################################################
Identifying the right ubuntu compute resource type to use for efficiency
identifying all the necessary libraries to be installed for a smooth testing
