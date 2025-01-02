# Ansible boilerplates

## Instructions

1. Open this repository in VSCode

2. Open Command Palette

3. Reopen this project in DevContainer

4. Create a `inventory.ini` file in the root folder with the following content (copy-pase `inventory.example.ini`)

```ini
[vps]
VPS_IP_ADDRESS ansible_user=VPS_USER ansible_ssh_pass=VPS_PASSWORD
```

5. Specify necessary configs in `.env.yaml` file

## Running playbooks

Execute the following code:

```bash
ansible-playbook path/to/playbook.yaml
```

## Testing connection

```bash
ansible all -m ping
```