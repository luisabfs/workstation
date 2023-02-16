# Workstation
Ansible playbook to ✨automagically✨ install my workstation tools.

>_Disclaimer:_  
These scripts are MacOS M1/Ubuntu related with major version 18+, for other distributions you'll need to adapt it.
Read the correspondent `.yaml` file before applying and be sure to understand everything that will be done.


## Steps
Type your password when asked to give root permissions for some actions.

### MacOS M1

1. Install XCode command line tools

```
xcode-select --install
```

2. Install Homebrew

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

3. Add Homebrew to your PATH
```
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/$YOUR_DEVICE_NAME/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

4. Install Ansible
```
brew install ansible
```

5. Clone this repository
```
git clone https://github.com/luisabfs/workstation.git
```

6. Apply the configuration
```
ansible-playbook workstation/macos.yaml --ask-become-pass
```

### Ubuntu

1. Install Ansible
```
sudo apt update && sudo apt install ansible unzip git -y
```

2. Clone this repository
```
git clone https://github.com/luisabfs/workstation.git
```

3. Apply the configuration
```
ansible-playbook workstation/ubuntu.yaml --ask-become-pass
```

## Links

- [Usando o Ansible para Automatizar minha Workstation - Caio Delgado [Youtube Video]](https://youtu.be/bG2kX7W_s0c)
- [Ansible Documentation](https://docs.ansible.com/)
