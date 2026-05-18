## Project: 
# `Provisioning and Management Automation of Multi-OS EC2 Instances using Ansible`

## About the Project

Built a cloud automation project using Ansible to automate the provisioning and management of AWS EC2 instances across multiple operating systems.

The project focuses on infrastructure automation, secure SSH-based communication, and conditional execution of tasks based on system facts collected from managed nodes.

---

## Project Workflow

This project demonstrates practical DevOps automation by performing the following operations:

- Automated provisioning of multiple AWS EC2 instances
- Secure passwordless SSH setup between control and managed nodes
- Conditional task execution using Ansible facts
- Automated infrastructure management using Ansible playbooks

---

## Automation Tasks Performed

### Task 1: EC2 Instance Provisioning

- Dynamically launched 3 EC2 instances using Ansible loops
  - 2 Ubuntu instances
  - 1 CentOS instance
- Eliminated repetitive configurations through loop-based automation

---

### Task 2: Passwordless Authentication-SSH

- Generated SSH key pair in the Ansible control node
- Shared public key with target EC2 instances
- Enabled secure passwordless remote connectivity

---

### Task 3: Stopping EC2 instances

- Implemented conditional automation using:

```yaml
when: ansible_facts['os_family'] == "Debian"
- This used to stop two Ubuntu insatnces.

- Shutdown task executed only on Ubuntu instances
- CentOS instance was excluded from shutdown operation

---

## Technologies & Services Used

- Ansible
- AWS EC2
- YAML
- SSH
- Linux

---

## Knowledge Gained

- Automating cloud infrastructure provisioning
- Using loops for scalable automation
- Applying conditional logic with `when`
- Managing multi-OS environments using Ansible facts
- Understanding idempotent infrastructure automation
- Handling real-time DevOps administration tasks
