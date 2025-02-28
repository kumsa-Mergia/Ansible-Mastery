# Ansible Roles Structure Best Practices

## 1. Organizing Roles

To create modular and reusable Ansible roles, it’s essential to follow a standardized structure. This allows for better management, scalability, and reuse of code.

**Recommended Role Directory Structure**:

```bash
roles/
├── <role_name>/
│   ├── defaults/
│   │   └── main.yml          # Default variables for the role
│   ├── files/                # Static files for the role
│   ├── handlers/             # Handlers (notifications, triggers, etc.)
│   │   └── main.yml
│   ├── meta/                 # Role metadata, including dependencies
│   │   └── main.yml
│   ├── tasks/                # Core tasks to be executed in the role
│   │   └── main.yml
│   ├── templates/            # Jinja2 templates used by the role
│   ├── tests/                # Test playbooks for validating the role
│   ├── vars/                 # Variables specific to the role
│   │   └── main.yml
│   └── README.md             # Documentation about the role
