# Ansible Vault: Secure Your Sensitive Data

Ansible Vault allows you to securely store and manage sensitive data such as passwords, API keys, and other confidential information. This ensures that secrets are not exposed in your playbooks or variables files.

## Key Features of Ansible Vault:
- **Encryption**: Encrypt sensitive files to prevent unauthorized access.
- **Decryption**: Decrypt files when needed during playbook execution.
- **Passphrase Protection**: Encrypt files with a passphrase that can be shared among trusted users.

## Encrypting a File:
To encrypt a file using Ansible Vault, use the following command:

```bash
ansible-vault encrypt <filename>
```
## Decrypting a File:
To decrypt a file, use the following command:

```bash
ansible-vault decrypt <filename>
```
## Using Encrypted Files in Playbooks:
You can use encrypted files in your playbooks by specifying the --ask-vault-pass or --vault-password-file option when running Ansible.

```bash
ansible-playbook site.yml --ask-vault-pass
```
## Alternatively, you can pass the vault password from a file:

```bash
ansible-playbook site.yml --vault-password-file ~/.vault_pass
```
