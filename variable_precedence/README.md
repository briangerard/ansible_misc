# Which Variables Clobber Which?

This is a play which tests which method of variable setting takes precedence
over which others, between the following methods:
  - Setting via 'vars' in the playbook.
  - Setting via included 'vars\_files' in the playbook.
  - Setting via 'group\_vars/all'
  - Setting via 'group\_vars/specific\_group'
  - Setting via '--extra-vars', on the ansible-playbook command line.

There is a template ('the\_file.j2') in the 'files' directory, which will end up
as /tmp/ansible\_variable\_precedence\_test.txt after all variables have been
expanded.

To run, simply execute ```./run_the_play``` in this directory.
