# ansible
# Install ansible
Apt (Ubuntu): sudo apt-get install -y ansible\n
Yum (CentOS): sudo yum install ansible\n
Mac: brew install ansible\n

# Check version
ansible --version

# Login whithoud password
ssh-keygen
ssh-copy-id username@webserver
Ex. ssh-copy-id jesse@128.107.241.178

# Ping the server on host
ansible -m ping all

# Pse shell function
ansible -m shell -a 'df -h' centos
ansible -m shell -a 'whoami' ucdavis

# Run the playbook
ansible-playbook -m -K main.yml

