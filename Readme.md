### What will this role do ?

The above package role will help you install various packages on the node or server that we want to prepare for our deployment of application on dcos.

This role will further run ntp and start the ntpd daemon as a service.



#### Variable used in the role.

- common_default_packages: ' This includes all the packages that this role installs.'

- common_pip_packages: - 'It would install the aws cli '
- common_removed_packages: - 'It is used for removing unwanted package chronyd.'

#### Prerequisite

- This role to be run on rhel/centos system.

### How to run the playbook .

To run the playbook follow the below command:-

`ansible-playbook -i <your inventory file> playbook.yml`

**Note**:-  If you are running on your local system then you don't need to pass inventory file. Just use localhost in hosts of playbook. 