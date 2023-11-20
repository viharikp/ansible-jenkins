## Jenkins Deployment Playbook 
- Ansible 
- Ubuntu OS - 22.04

## To Deploy Jenkins Server
1. Edit the inventory file, under [jenkins] add ip addresses for the servers along with the role_type
2. Run the playbook: ansible-playbook -i inventory/inventory.ini jenkins_playbook.yml

## To Deploy HAProxy Server
1. Edit the inventory file, under [proxies], add the ip address for the servers along with the jenkins_server
2. Add the Virtual IP address to group/all/vars
3. Run the playbook: ansible-playbook -i inventory/inventory.ini haproxy_playbook.yml
