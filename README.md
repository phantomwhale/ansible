# Mac Development Ansible Playbook

This playbook should install and configures most of the software I use on my Mac for software development. It's currently a work in progress, extracting this functionality from install scripts in my dotfiles repo.

## Installation

1. Ensure Apple's command line tools are installed (`xcode-select --install` to launch the installer).
2. [Install Ansible](https://docs.ansible.com/ansible/latest/installation_guide/index.html):

   1. Install Ansible: `python3 -m pip install --user ansible`

3. Clone or download this repository to your local drive.
4. Run `~/Library/Python/3.9/bin/ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible roles.
5. Run `~/Library/Python/3.9/bin/ansible-playbook --ask-become-pass --ask-vault-pass local.yml` inside this directory. Enter macOS account password when prompted for the 'BECOME' password.

> Note: If Homebrew commands fail, might need to agree to Xcode's license or fix some other Brew issue. Run `brew doctor` to see if this is the case.

## Reference

Much of the Ansible work builds on top of the useful roles and collections shared by [Jeff Geerling](https://github.com/geerlingguy), namely <https://github.com/geerlingguy/ansible-collection-mac>
