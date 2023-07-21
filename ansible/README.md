# ansible

This directory contains Ansible code for bootstrapping a Foreman/Katello server.

## Usage

Edit the [`lab-inventory.ini`](lab-inventory.ini) inventory to match your server's connection details.

Rename/copy the [`host_vars/00-foreman.sva.de`](host_vars/00-foreman.sva.de) directory to match your server's name. Also, edit [`credentials.yml`](host_vars/00-foreman.sva.de/credentials.yml) in that directory.

If needed, edit [`group_vars/foreman/foreman.yml`](group_vars/foreman/foreman.yml) and [`group_vars/foreman/storage.yml`](group_vars/foreman/storage.yml) to define software content to synchronize and storage devices to use.

Run the playbook:

```command
$ ansible-playbook -i lab-inventory.ini -K
```
