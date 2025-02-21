# Lab 7 Ansible


![image](https://github.com/user-attachments/assets/cb690291-7dff-4951-a323-807e80539fc4)
![image](https://github.com/user-attachments/assets/155a915c-7643-457e-be33-79d49c3c6ec7)

## Create Key
```bash
ssh-keygen -t rsa -C "aws" -f ~/.ssh/aws
```

## Push changes and run Ansible Playbook
```bash
ansible-playbook playbook.yml
```

```yml
# Name of the ansible block (generally a description of what the block does)
    - name: create link to nginx config file to enable it
# Call to the file module in ansible
      ansible.builtin.file:
# This will set a symbolic link from the default file in /etc/nginx/sites-available to /etc/nginx/sites-enabled/default
        src: /etc/nginx/sites-available/default
        dest: /etc/nginx/sites-enabled/default
# States that the module will use a symbolic link
        state: link
```
