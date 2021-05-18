# Readme

Magento Add Admin User via Ansible

## Prerequisite

Copy the "hosts.yml.sample" and create "hosts.yml"

```
cp hosts.yml.sample hosts.yml
```

Then update the `ansible_user` and `ansible_host` entries for each instance.

## Invocation:

Run:

```
ansible-playbook magento_add_admin_user.yml -e "target:<name_of_the_instance_from_hosts.yml>"
```

## Warning

Test this on a non-live environment.

Please kindly read and review the following files:

- hosts.yml
- magento_add_admin_user.yml
- group_vars/user_vars.yml
- roles/magento_add_admin/tasks/magento_add_admin_user_task.yml

Proceed at your own risk.

## ToDo

- Not sure!!

## Reference

This ansible snipper is created by refering "ansible/ansible-examples".
Especially the https://github.com/ansible/ansible-examples/tree/master/lamp_simple

### Other References:

- https://www.edureka.co/community/36502/execute-shell-commands-using-ansible
- https://docs.ansible.com/ansible/2.4/shell_module.html
- https://stackoverflow.com/questions/32704247/ansible-variable-within-variable
