# Delta Blue - Ansible Odoo Deployment

## SSH access to private Git projects/repositories

The option `odoo_user_generate_ssh_key` ensures a SSH key shall be generated for the Odoo system user (`odoo_user`)

The first time executing the Ansible Playbook it shall crash, due to SSH access error.
Get the SSH public-key from the log output and add as Deploy Key to the necessary Git projects.
Run the Ansible Playbook again, which now should pass the Git clone actions.
