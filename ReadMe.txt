This is the task for MSRCOSMOS.
Task 1: 
    AWS.YML
    This is a ansible playbook which will launch 2 ec2 instances naming msr-test-instance-1 and msr-test-instance-2
    
Task 2:

    packages.yml
     
     This playbook will install all the software packages of NVM Node Docker Docker Compose Openssl and Git.

Task 3:

    docker-compose.yml
      This file will install the apache service in the MSR-test-instance-1 and will set the port to access via web
      
    automatedeploy.yml
      This ansible playbook will check what are the containers running and will get a test.html file from github and save it in source
      once this is done by using git module we change the location of the file from source to destination(/var/www/html)and then you can access UI
      to see the webresult.
Task 4:
     db.yml
     This ansible playbook will install the sofware properties first and then installs the necessary PPA source packages and then will
      install the couchdb software.Once this is done change the permissions to couchdb and give all the access.once this is done start the 
      couchdb service.
      Once this is done you can access the db by giving a command
      $ curl localhost:5984
      
Task 5:
     ReadMe.txt
     This file gives all the documentation of the tasks performed.
     
Task 6:
    All the ansible files are self explanatory as name is defined for each module and for doing this you have to run these playbooks 
    on a machine where ansible is installed and inventory details are given properly.
      
    
    
