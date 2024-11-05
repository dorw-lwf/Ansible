# Ansible

## Ad-hoc commands
ad hoc tasks can be used to reboot servers, copy files, manage packages and users, and much more. You can use any Ansible module in an ad hoc task. ad hoc tasks, like playbooks, use a declarative model, calculating and executing the actions required to reach a specified final state. They achieve a form of idempotence by checking the current state before they begin and doing nothing unless the current state is different from the specified final state.

Use ansible Ad-hod commands for example to copy files to remote grouped hosts:
```bash
$ ansible uk -m ansible.builtin.copy -a "src=/etc/hosts dest=/tmp/hosts"
```