User n Group Management
=========

A brief description of the role goes here.

Requirements
------------

Python2.7 on the nodes

Role Variables
--------------

Update role variables as required in `vars/main.yml`

Example Playbook
----------------

Include the role in playbook (eg. user.yml) as defined:

    - hosts: nodes
      roles:
         - { role: user-mgmt }

Playbook Execution
----------------

Execute the playbook using the below command with required vars (playbook name: user.yml):

    ansible-playbook user.yml -e "PROJECT=myproject1 ENV=dev"

