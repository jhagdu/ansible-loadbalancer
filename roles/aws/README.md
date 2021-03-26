AWS
===

Ansible Role to create a AWS Infrastructure for HAProxy and Webservers

Requirements
------------

AWSCLIv2 should be installed and configured  
  
Required Python Packages -  
- boto  
- boto3  
- botocore  
- python >= 2.6  

Role Variables
--------------

Variables which should be included in additional variable files or vault -  

    aws_access_id: AWSACCESSIDHERE
    aws_access_secret_key: AWSACCESSSECRETKEYHERE


Variables in vars/main.yml -  

    region: ap-south-1
    inst_type: t2.micro
    ami_id: ami-09a7bndj88a6alfif
    subnet_id: subnet-8aefg5ed

Dependencies
------------

No Dependencies on other roles or collections

Example Playbook
----------------

aws-login.yml is a additional variable file or vault that contains required variables -

    - hosts: servers
      vars_files:
         - aws-login.yml
      roles:
         - aws

License
-------

BSD

Author Information
------------------

Author Name: Aman Jhagrolia  
Contact: https://www.linkedin.com/in/amanjhagrolia143  
