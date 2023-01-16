# Workstation
Ansible playbook to ✨automagically✨ install my workstation tools.

>Disclaimer:
Those scripts are ubuntu related with major version 18+, for other distributions you'll need to adapt it

## Steps
> Read the pop!_os.yaml file before applying and be sure to understand everything that will be done.

1. Install Ansible
`sudo apt update && sudo apt install ansible unzip git -y`

2. Clone this repository
`git clone https://github.com/caiodelgadonew/tools.git`

3. Apply the configuration
`ansible-playbook tools/ubuntu.yml --ask-become-pass`

Type your password when asked to give root permissions for some actions.

## Links

- [Usando o Ansible para Automatizar minha Workstation - Caio Delgado [Youtube Video]](https://youtu.be/bG2kX7W_s0c)
- [Ansible Documentation](https://docs.ansible.com/)
