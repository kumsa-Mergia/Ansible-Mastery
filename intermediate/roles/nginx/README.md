# Ansible Role Directory Structure

=======================================================
When you run the command:

```sh
ansible-galaxy init nginx
```

Ansible automatically generates a role directory structure. This structure ensures that your role is well-organized and follows best practices.

## Directory Structure

- **`defaults/`** – Contains the default values for role variables.
- **`files/`** – Holds static files that may be copied to the target system.
- **`handlers/`** – Contains handler tasks that are triggered by other tasks.
- **`meta/`** – Defines metadata for the role, such as dependencies, author, license, etc.
- **`tasks/`** – Contains the main tasks of the role.
- **`templates/`** – Holds Jinja2 templates that will be rendered and placed on the target system.
- **`vars/`** – Contains variables that are typically more static and non-overridable.

This structure helps maintain clean, reusable, and scalable Ansible roles.

