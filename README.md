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
