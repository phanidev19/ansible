# Ansible
## Prerequisites:
*  Install Ansible
*  Install Python
*  Uncomment the below line in file `/etc/ansible/ansible.cfg`
     ```shell script
      host_key_checking = False
      ```
## Ansible useful commands
* To check connectivity
   ```shell script
    ansible smarthome -i hosts -m ping
   ```
* To list hosts
   ```shell script
    ansible smarthome -i hosts --list-hosts
   ```
* To check ansible playbook syntax
   ```shell script
    ansible-playbook -i inventories/hosts deploy.yml --syntax-check
   ```
  
* To execute a playbook
   ```shell script
    ansible-playbook -i inventories/hosts deploy.yml --extra-vars "hosts=smarthome"
   ```

    
   
   
