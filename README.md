# wca-ansible
Ansible repository with sample prompts to generate Ansible content leveraging IBM Watsonx Code Assistant(WCA) for Red Hat Ansible Lightspeed.

# Overview
There are 2 ansible playbooks in this repository. These playbooks have prompts required to generate ansible content as per desired task. WCA for Ansible Lightspeed can be leveraged to generate Ansible code in this playbook.

`create-aws-infra.yml` playbook is used to deploy the infrastructure as depicted in the below diagram. The playbook is initialized with an existing VPC ID and subnet details. Security groups for Application load balancer(ALB), EC2 instances are created first. Followed by it, 2 EC2 instances are deployed. Next a target group is created with these EC2 instances as targets and ALB is created with this target group. 


![image](https://github.com/dimallya/wca-ansible/assets/99815425/7b7aa8c2-3b8b-460f-8add-67eb6d92a7d6)



`deploy-webserver` playbook is used to deploy webserver on the target hosts i.e. 2 EC2 instances deployed in earlier step. 


