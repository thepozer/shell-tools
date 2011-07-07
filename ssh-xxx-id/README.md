# ssh-xxx-id commands
The main goal of these command is to work with more than one ssh host.

## ssh-cp-id 
This command is based on ssh-copy-id with the posibility to copy the public key on more than one ssh host.

_Usage_
    ssh-cp-id [-i public_key_file] user@ssh_host [user1@ssh_host1] [user2@ssh_host2] ...

## ssh-ls-id 
This command list all key's email found in the authorized_keys file oh the ssh hosts.
The list is splitted by ssh host.

_Usage_
    ssh-cp-id 'key_email' user@ssh_host [user1@ssh_host1] [user2@ssh_host2] ...

## ssh-find-id 
This command search if the key's email is in the authorized_keys file oh the ssh hosts.

_Usage_
    ssh-cp-id 'key_email' user@ssh_host [user1@ssh_host1] [user2@ssh_host2] ...

## ssh-rm-id 
This command remove the key linked to the key's email, if this one is in the authorized_keys file oh the ssh hosts.

_Usage_
    ssh-rm-id 'key_email' user@ssh_host [user1@ssh_host1] [user2@ssh_host2] ...



