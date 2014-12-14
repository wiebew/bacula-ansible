bacula-ansible
==============

install bacula client and server with ansible


Currently assumes one remote client


you could generate a password with: 
```console
openssl rand -base64 32 | tr -cd '[:alnum:]'
console


On Apple OSX this will paste in your clipboard
```console
openssl rand -base64 32 | tr -cd '[:alnum:]' | pbcopy
console

