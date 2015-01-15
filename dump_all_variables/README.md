# What Variables Does Ansible Have?

The purpose of this playbook is just to dump all the variables Ansible knows
about to /tmp/ansible.all.variables

The template and final task in the playbook can be inserted into other playbooks
for debugging purposes (trying to track down if a variable is not being set or
is being overwritten, for instance).  This is more a proof-of-concept than
anything, though it can be illustrative of where Ansible keeps various bits of
data.

To run, simply execute ```./run_the_play``` in this directory.
