## A playbook for testing ```become``` as well as getting vars from the vaulted vars file.

I have troube on MacOS to get ```ansible_become_password``` working - interestingly, it works as expected on Ubuntu, but on MacOS it chokes. This, as well as googling a lot only to find out that there aren't a lot of examples on how to get your password and use it made me write this simple playbook. 

To use it, you need the vars file ```inventory/group_vars/local``` and it should look something like this:
```
---
vault_ansible_become_password: <password>
vault_var1: Success!
```
