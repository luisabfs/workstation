# Workstation
Ansible playbook to ✨automagically✨ install my workstation tools.

>_Disclaimer:_  
These scripts are Ubuntu related with major version 18+, for other distributions you'll need to adapt it.


## Steps
> Read the ubuntu.yaml file before applying and be sure to understand everything that will be done.

1. Install Ansible
`sudo apt update && sudo apt install ansible unzip git -y`

2. Clone this repository
`git clone https://github.com/luisabfs/workstation.git`

3. Apply the configuration
`ansible-playbook worksation/ubuntu.yaml --ask-become-pass`

Type your password when asked to give root permissions for some actions.

## Links

- [Usando o Ansible para Automatizar minha Workstation - Caio Delgado [Youtube Video]](https://youtu.be/bG2kX7W_s0c)
- [Ansible Documentation](https://docs.ansible.com/)
