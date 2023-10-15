# Project Deployment Readme

This repository contains scripts for deploying a node application using Ansible. 

## Prerequisites
- Ansible installed on the deployment machine

## Instructions

    ansible-playbook -i hosts deploy-node.yaml

This command executes the Ansible playbook `deploy-node.yaml` using the inventory file `hosts`. The playbook likely contains instructions for deploying a node application to a specified set of hosts. Make sure to set the hosts correctly in the inventory file before executing this command.

    ansible-playbook -i hosts deploy-node.yaml -e "version=1.0.0 location=/home linux_name=souhail"

This command is similar to the previous one but with extra parameters passed using the `-e` flag. It specifies the version of the application (`version=1.0.0`), the deployment location (`location=/home`), and the name of the Linux system (`linux_name=souhail`). Adjust the values according to your specific deployment requirements.

    ansible-playbook deploy-node.yaml

This command assumes that the `hosts` file is already configured and the playbook `deploy-node.yaml` contains the necessary configuration for the deployment. Ensure that the playbook is properly configured before executing this command.

Note: Make sure to customize the `deploy-node.yaml` playbook and the `hosts` file according to your specific project requirements and target environment.

For any issues or questions, please reach out to the project maintainers.

