# ansible
## Install ansible
Apt (Ubuntu):  
```
sudo apt-get install -y ansible
```

Yum (CentOS): 
```
sudo yum install ansible
```
Mac: 
```
brew install ansible
```

## Check version
```
ansible --version
```

## Login whithoud password
Generating public & private keys
```
ssh-keygen
```
Put the public key to server <br />
Ex. ssh-copy-id jesse@128.107.241.178
```
ssh-copy-id username@webserver
```

## Ping the server on host
```
ansible -m ping all
```

## Use shell function
Check the disk condition
```
ansible -m shell -a 'df -h' centos
```
Check the user name
```
ansible -m shell -a 'whoami' ucdavis
```

## Run the playbook
Run main.yml
```
ansible-playbook -m -K main.yml
```
