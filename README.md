# wca-ansible
Ansible repository with sample prompts to generate Ansible content leveraging WCA for Ansible Lightspeed.

# Overview
There are 2 ansible playbooks in this repository. These playbooks have prompts required to generate ansible content as per desired task. IBM Watsonx Code Assistant for Ansible Lightspeed can be leveraged to generate Ansible code in this playbook.

`create-aws-infra.yml` playbook is used to deploy the infrastructure as depicted in the below diagram. The playbook is initialized with an existing VPC id and subnet details. Security groups for Application load balancer, EC2 instances are created first followed by it, 2 EC2 instances are deployed. Next a target group is created with these EC2 instances as targets and ALB is created with this target group. 

`deploy-webserver` playbook is used to deploy webserver on the EC2 instances. 


![image](https://github.com/dimallya/wca-ansible/assets/99815425/7b7aa8c2-3b8b-460f-8add-67eb6d92a7d6)


