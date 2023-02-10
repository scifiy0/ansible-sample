<!--  -->

## Sample Ansible Configuration

Repo contain sample playbook to get started and try with ansible

------
> ### *** this playbook will check which distro that nodes belong to and deploy, start sample nginx webserver with default configuration ,
------
To get start : 
``` 
in the inventories files modify or add worker-nodes ip address.
we can add more nodes by appending label under hosts:
    hosts:
        ...
        node3-<os-distro>: 
            ansible_host: IP-ADDRES-HERE

```

------
running this playbook by issuing the command:
```
ansible-playbook -i inventories/inventory.yml ws.yml -k -u <user>
```

------
