# infra-jenkins
Create &amp; Setup GitHub Repository for Jenkins Ansible Playbooks

| Name                | NUID      | Email                          |
| ------------------- | --------- | ------------------------------ |
| Ketki Kule          | 001549838 | kule.k@northeastern.edu        |
| Sandeep Wagh        | 001839964 | wagh.sn@northeastern.edu       |
| Vignesh Gunasekaran | 001029530 | gunasekaran.v@northeastern.edu |


## To run the playbook :

ansible-playbook -v -e aws_profile=root -e key_name=csye7125 -e ami_id=ami-id -e tag_value=jenkins -e elastic_ip=54.xx.yy.zzz networking-setup-playbook.yml


ansible-playbook -vvvv -e domain_name=domain -e key_name=key -e email_id=email software-setup-playbook.yml


ansible-playbook -vvvv -e user_name=admin -e password=admin -e user_id=jenkins -e tag_value=jenkins jenkins-plugin-playbook.yml



ansible-playbook -vvvv -e user_name=admin -e password=admin -e tag_value=jenkins -e download_url=http://localhost:8080/jnlpJars/jenkins-cli.jar -e github_username=username -e github_token=token -e github_repo=helm-chart  -e github_org=cyse7125-fall2022-group03 -e user_id=jenkins -e job_name=jenkinsJob jenkins-job-playbook.yml



## To kill the instance:

ansible-playbook -v -e aws_profile=dev -e key_name=key -e tag_value=jenkins -e vpc_name=vpc_jenkins-us-east1 network-termination-playbook.yml




 
