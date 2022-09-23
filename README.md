# infra-jenkins
Create &amp; Setup GitHub Repository for Jenkins Ansible Playbooks


## To run the playbook :

ansible-playbook -v -e aws_profile=root -e key_name=csye7125 -e ami_id=ami-09af0000000094909 -e tag_value=jenkins -e elastic_ip=aa.bb.ccc.dd networking-setup-playbook.yml


## To kill the instance:

 ansible-playbook -v -e tag_value=jenkins -e aws_profile=root network-termination-playbook.yml 
