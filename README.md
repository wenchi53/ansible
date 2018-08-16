# ansible

# Login whithoud password
ssh-keygen
ssh-copy-id username@webserver
# ssh-copy-id jesse@128.107.241.178

# ping the server on host
ansible -m ping all

# use shell function
ansible -m shell -a 'df -h' centos
ansible -m shell -a 'whoami' ucdavis

# Run the playbook
ansible-playbook -m -K main.yml

