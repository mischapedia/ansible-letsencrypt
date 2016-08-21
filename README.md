Ansible playbook to setup HTTPS using Let's encrypt on nginx.

This provides a server capable of serving static files using HTTPS.

To use:
 1. Install [Ansible](https://www.ansible.com/)
 2. Setup a server accessible over ssh
 3. Create /etc/ansible/hosts according to template below and change example.com to your domain
 4. Copy the rest of the files to an empty directory (`playbook.yml` in the root of that folder and the rest in the `templates` subfolder)
 5. Run `ansible-playbook playbook.yml`
 6. Copy your (static HTML) code to `/var/www/example.com` (`example.com` replaced with your domain)