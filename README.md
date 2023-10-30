# Ansible-Tutorial

This repository contains Ansible playbooks and configuration files to automate the deployment and management of an Apache web server on an EC2 instance. This README provides an overview of the project, instructions on how to use it, and common issues you may encounter.

## Overview

The purpose of this project is to simplify the process of deploying and managing an Apache web server on an Amazon EC2 instance using Ansible. It streamlines the setup and configuration, making it a straightforward process.

## Prerequisites

Before you begin, ensure you have the following prerequisites:

- Ansible installed on your local machine.
- An AWS account.
- An EC2 instance created in your AWS account.

## Getting Started

1. **Clone the Repository:**

   ```bash
   https://github.com/anant996/Ansible-Tutorial.git

2. **Run the Ansible Playbook:**

   Execute the Ansible playbook to install and manage Apache:

   ```bash
   ansible-playbook -i inventory.yml apache.yml
The playbook will install Apache on your EC2 instance.

## Accessing Your Apache Server
Once the playbook has run successfully, you can access your Apache server by navigating to your EC2 instance's public IP address in your web browser.

## Common Issues
   If you encounter any issues during the setup and execution of this project, here are some common problems and their solutions:

   1. Issue: Locale Encoding Error<br>
      Solution: Set your locale encoding to UTF-8. You can do this by running the following command:<br>
      ```bash
      export LC_ALL=C.UTF-8
      export LANG=C.UTF-8
      
   2. Issue: Authentication Error<br>
      Solution: Make sure to provide the correct SSH private key file path in the apache.yml file.<br>
      Example: ansible_ssh_private_key_file: "/path/to/your/your_pem_file.pem"<br>

Add any other common issues you encountered and their solutions here. 

## Does Ansible work with Windows   
Yes, Ansible can run on Windows, but it has certain limitations and considerations due to its primarily Unix-based design.<br>
For detailed installation refer to [TutorialsPoint](https://www.tutorialspoint.com/how-to-install-and-configure-ansible-on-windows).

## References
   Official Documentation: https://docs.ansible.com/ansible/latest/index.html<br>
   Blog: https://linuxopsys.com/topics/ansible-playbook-to-install-apache<br>
   Blog: https://www.freecodecamp.org/news/what-is-ansible/


