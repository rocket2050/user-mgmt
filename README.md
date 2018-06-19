
User n Group Management
=========

This role will generate the key_pair in localhost and then it will create users and groups in all nodes.

Requirements
------------

Python2.7 on the nodes

Role Variables
--------------

Update role variables as required in `vars/main.yml`

Example Playbook
----------------

Include the role in playbook (eg. users.yml) as defined:

- hosts: '{{ TARGET }}'

  roles:
  - user-mgmt

Playbook Execution
----------------

Execute the playbook using the below command with required vars (playbook name: users.yml):

 ```  (To generate key_pair) : ansible-playbook users.yml -e "ENV=dev TARGET=localhost" --tags "key_mgmt" ```
 
 ```  (To create users and groups) : ansible-playbook users.yml -e "ENV=dev TARGET=node1" --tags "user_mgmt" ```
