# bacula-ansible

install bacula client and server with ansible

Currently assumes one remote client. Client has a running mysql database. The database credentials are stored in /root/.my.conf. This script is meant for the server created by the https://github.com/wiebew/ispconfig_install ansible script

#### Usage
create vars.yml file, copy it from vars.yml.example 
fill in the values.

to generate a strong password: 
```console
openssl rand -base64 32 | tr -cd '[:alnum:]'
```

On Apple OSX this will paste the password in your clipboard, so you can paste it in the editor:
```console
openssl rand -base64 32 | tr -cd '[:alnum:]' | pbcopy
```

create the hosts file, copy it from hosts.example
fill in the values. 

run the script with:

```console
ansible-playbook -i hosts playbook.yml
```




