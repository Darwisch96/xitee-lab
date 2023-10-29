# This playbook is meant to

- install required ansible collections for the playbook.
- Create user xitest with sudo priviledges.
- Install Wordpress web application.
- Configure Firewall to make sure wordpress is accessible and up and runing with high availability using permanent databse. 
- Create Cronjob to backup wordpress mysql database files 

# RUN: 

$ ./install_ansible_collections.sh && ansible-playbook xitee-homework.yml


# Check wordpress is up and running 
$ podman ps 
$ curl -kv http://127.0.0.1:8080
