# Ansible playbook for setup Host-based SSH

## Configuration

```ini
[server]
ssh.server.who.receive.connections

[client]
ssh.client.who.connects

[client:vars]
allowed_domain=domain.com
```

**Disclaimer: A host can be server and client at the same time.**

## Usage

```
ansible-playbook -i inventory.ini main.yml
```