# infra-jenkins
Create &amp; Setup GitHub Repository for Jenkins Ansible Playbooks


## To run the playbook :

ansible-playbook -v -e aws_profile=root -e key_name=csye7125 -e ami_id=ami-09af0000000094909 -e tag_value=jenkins -e elastic_ip=aa.bb.ccc.dd networking-setup-playbook.yml


## To kill the instance:

 ansible-playbook -vvvv -e aws_profile=dev -e tag_value=jenkins -e vpc_name=vpc_jenkins-us-east-1 network-termination-playbook.yml 
 
