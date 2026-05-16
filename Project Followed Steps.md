# Steps followed in this project 
Required Prerequirties
-
 - 1: Install Ansible -  [Ansible](https://docs.ansible.com/projects/ansible/latest/installation_guide/intro_installation.html) - Click this link and follow guidelines to install ansible

 - 2: Install Boto3 - `pip install boto3`
 - 3: Install AWS Collection - `ansible-galaxy collection install amazon.aws`
----
### Task 1- Provisioning three EC2 instances using Ansible loops

#### Step 1. 
 - Open IAM in AWS. Create a user, attach `Ec2 full access` policy in it.
 - Generate API keys which to be secure in Ansible Vault.

#### Step 2.
 - Create an Ansible YAML playbook which is to provision and manage the three AWS EC2 instances.
 - Here `loop` is used to iterate the three Ec2 instances.
 - From Ansible Documentation, we can use the example playbooks or we can create our own playbooks according to our need.

 ##### Playbook:
  <img width="663" height="390" alt="image" src="https://github.com/user-attachments/assets/b852c8b9-b3c2-4418-b64b-119e531b2580" />

#### Step 3.
 - Ansible vault is created to store our API keys- Access key and secret key.
 - Below commands used to create vault to store keys.
   <img width="1055" height="92" alt="vault" src="https://github.com/user-attachments/assets/76543bd8-77a5-4527-bf62-ccf354618603" />

#### Step 4.
 - Executing our playbook.

   <img width="1354" height="333" alt="run playbook" src="https://github.com/user-attachments/assets/c0f299d8-ccba-4959-ac75-80be9bb5326b" />

#### Step 5.
- Verify AWS EC2 Instances. Here the provisioned 2 Ubuntu and 1 CentOs EC2 instances are created successfully.

  <img width="1297" height="346" alt="3ec2instances" src="https://github.com/user-attachments/assets/806e0717-eea2-4753-bb53-5add55d83fd8" />



