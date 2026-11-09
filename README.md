# Terraform & Ansible

## Terraform

### Docker

```bash
cd terraform/docker
terraform init
terraform plan
terraform apply
```

Nginx accessible sur http://localhost:8000

### AWS

```bash
cd terraform/aws
terraform init
terraform plan -var="my_ip=<mon_ip>"
terraform apply -var="my_ip=<mon_ip>"
```

## Ansible

```bash
cd ansible
ansible all -i hosts -m ping
ansible-playbook --syntax-check deploy.yml
ansible-playbook -i hosts deploy.yml
```
