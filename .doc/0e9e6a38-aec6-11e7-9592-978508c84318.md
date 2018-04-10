[README](/) / [Technical](0e9eb851-aec6-11e7-9592-978508c84318.md) / [Getting Started](0e9eb852-aec6-11e7-9592-978508c84318.md) / [Environment](0e9eb853-aec6-11e7-9592-978508c84318.md) / [Set up environment](0e9e6a38-aec6-11e7-9592-978508c84318.md)

# tuningfork-ansible

## Installation

### Verify requirements and install Ansible

#### Upgrade pip version

```bash
$ pip install --upgrade pip
```

#### Install Ansible and requirements

```bash
$ pip install -r requirements.txt
```

This command will install specific Ansible version.

#### Verify Ansible version

```bash
$ ansible --version
```

Should show something like

```
ansible 2.3.2.0
  config file =
  configured module search path = Default w/o overrides
```

## Initialize Vault

Ansible Vault stores sensitive data like MySQL credentials into an encrypted file.
Ansible automatically retrieve the passphrase from the MacOS keychain, but it needs to be added manually.

```bash
security add-generic-password -a ansible_vault_tuningfork-ansible -s ansible -w  P@SsW0rd_0N_l@s|PaSs
```

## Basic usage

### Configure all servers

```bash
ansible-playbook -i inventories/staging/hosts.ini servers.yml
```

### Deploy

```bash
ansible-playbook -i inventories/staging/hosts.ini deploy.yml
```
