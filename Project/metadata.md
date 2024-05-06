Pre-requesites: Set-up 'Ansible-cluster' and install 'Jenkins' in it.

=======
STEP: 1
=======
* Write Playbook in '/etc/ansible' Path and also copy the script.sh in this Path.
  NOTE: Make sure that all the Paths specified in playbook are correct.

=======
STEP: 2
=======
* Install plugins: ansible, deploy to container

=======
STEP: 3
=======
* Add ansible as tool: Dashboard-->Manage Jenkins-->Tools-->Ansible installations-->Add Ansible-->Name(ansible)-->Path to ansible executables directory(/usr/bin)-->save

=======
STEP: 4
=======
* Pipeline syntax: Sample Step(ansiblePlaybook:invoke an ansible playbook)-->Ansible tool(ansible)-->Playbook file path in workspace(/etc/ansible/playbook.yml)-->Inventory file path in workspace(/etc/ansible/hosts)-->SSH connection credentials(username and password(give credentials that you created while ansible set-up))-->Disable the host SSH key check(select it)-->Generate Pipline Syntax

=======
STEP: 5
=======
* Write Pipeline and make sure to add all the stages correctly.

