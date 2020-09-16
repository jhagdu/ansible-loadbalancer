# Ansible LoadBalancer  
This Repository Contains YML Code of Ansible Playbook to configure a Webserver on Instance Dynamically launched on AWS Cloud and then configure a LoadBalancer to balance load between them

 
# To Use :-
- Pull or Download this Repository and then create a create ansible vault named "aws-login.yml" and put your aws_access_id and aws_access_secret_key in that.

- After that Copy my ansible folder in you /etc/ directory  
  OR  
  Copy my ansible configuration only and make a groups named "webserver" and "loadbalancer" in your own inventory and also update configration file accordingly  
  
- After that Run the ansible playbook and you Webserver is Ready on your AWS with LoadBalancer 
