# Terraform Role for Ansible

This role installs a given version of Terraform

## Variables

Here is an example variables file.

```
terraform:
  version: 0.11.0
  url: https://releases.hashicorp.com/terraform/{{ terraform.version }}/terraform_{{ terraform.version }}_linux_amd64.zip
```

## Handlers

None.

## Example task with role

```
- name: Install Terraform
  hosts: all
  roles:
    - edr.terraform
```
