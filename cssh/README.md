# cssh command
The main goal of this command is to access to ssh host.

## cssh
This command is based on ssh-copy-id with the posibility to copy the public key on more than one ssh host.

_Usage_
    cssh [-h|--help] [-l|--list] [-c company] [username]

_Parameters_
	-c "company" : List only host link to "company"

	-l | --list  : Don't show dialog box but the list of host with the username (useful cssh-xxx-id scripts)
	
	-h | --help  : Show command usage 

_Global Variable_

	sSshUser     : Default username for the script (if nothing defined, it use www)

## Configuration file : ~/.ssh/servers.list
This configuration file is in XML. 

example : 
```xml
<servers>
    <server><company>Company</company><host>server1.company.com</host></server>
    <server><company>Company</company><host>server2.company.com</host></server>
    <server><company>Other Company</company><host>server1.other-company.com</host></server>
</servers>
```

