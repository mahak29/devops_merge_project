# devops_merge_project


This project deliver the information about the fast forward merging concept in Github with the use of # Jenkins.
So in this project I created two environments using docker image
    1. testing environment
    2. production environment
  
 The environments are maintained by jenkins automatically
 
 PRE-REQUISITES
        - Base OS (Windows) and RHEL8 (Vitual OS)
        - Docker inside RHEL8 and git bash in Windows 
        - Start the docker and stop the firewall so as to connect to the outside world
        - Installed ngrok in RHEL8 for the client connectivity
   
 Problem Statement
 - JOB1 : If Developer push to feature branch then Jenkins will auto fetch from feature branch and deploy on test-docker environment.
 
 - JOB2 : If Developer push to master branch then Jenkins will auto fetch from master and deploy on production-docker environment.
          Both the testing and production enviroment are on different docker environments
          
 - JOB3 : Jenkins will check (test) for the website running in test-docker environment. 
          If QAT approved then Jenkins will merge the feature branch to master branch and trigger job 2
          
 





   
