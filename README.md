## Standalone JBoss Deployment 

[![AnsibleTest](https://github.com/spy86/ansible-jboss-standalone/actions/workflows/main.yml/badge.svg)](https://github.com/spy86/ansible-jboss-standalone/actions/workflows/main.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

- Requires Ansible 1.2 or newer
- Expects CentOS/RHEL 6 or 7 hosts

This playbooks deploy a very basic implementation of JBoss ver 7.1 

    To run this playbook execute this commend :
    ansible-playbook -i hosts site.yml
    
## Application deployment

Second playbook deploy-application.yml which may be used to deploy the HelloWorld and Ticket Monster applications to JBoss hosts

    To run this playbook execute this commend :
    ansible-playbook -i hosts deploy-application.yml
    
HelloWorld application will be available at `http://<jboss server>:<http_port>/helloworld`
Ticket Monster application will be available at `http://<jboss server>:<http_port>/ticket-monster`

## Provision for AWS 

Third playbook which provided, example, to provision hosts in preparation for running this JBoss deployment.

    To run this playbook execute this commend :
    ansible-playbook -i hosts demo-aws-launch.yml

