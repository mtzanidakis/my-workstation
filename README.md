# Ansible provision for my workstation

## Usage

On a fresh Fedora Workstation installation, upgrade the system and then run:

```
bash bootstap.sh
ansible-playbook -K main.yml
```

Playbooks are grouped by categories in `playbooks` dir. The playbook `main.yml` is a wrapper for running all playbooks at once. To run specific playbooks pass their filenames to `ansible-playbook`, eg.

```
ansible-playbook -K playbooks/go.yml playbooks/user.yml
```

## Compatibility

Tested on Fedora Workstation 36.
