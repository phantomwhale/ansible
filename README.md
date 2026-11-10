# Mac Development Ansible Playbook

This playbook should install and configures most of the software I use on my Mac for software development. It's currently a work in progress, extracting this functionality from install scripts in my dotfiles repo.

## Installation

1. Install [Homebrew](https://brew.sh) with its official installer. This also installs Apple's Command Line Tools:

   ```sh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. Install Ansible: `/opt/homebrew/bin/brew install ansible`
3. Clone or download this repository to your local drive.
4. Run `/opt/homebrew/bin/ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible collections.
5. Run `/opt/homebrew/bin/ansible-playbook --ask-vault-pass local.yml` inside this directory. No task needs `sudo`, so there is no 'BECOME' password prompt.

Full paths are used because the shell isn't set up for Homebrew until the dotfiles are installed.

The playbook installs everything else from the `Brewfile`, but never upgrades outdated packages (upgrades that need `sudo` can't prompt from inside Ansible). Upgrade interactively with `brew bundle upgrade` or `brew upgrade`.

> Note: If Homebrew commands fail, might need to agree to Xcode's license or fix some other Brew issue. Run `brew doctor` to see if this is the case.

## Reference

Originally built on [Jeff Geerling](https://github.com/geerlingguy)'s <https://github.com/geerlingguy/ansible-collection-mac>; Homebrew is now installed during bootstrap and the playbook only applies the `Brewfile`.

## Manual Steps

> An incomplete, inexact and inaccurate list of other steps needed post-install that I haven't, can't or won't automate

Install youtube-music: https://github.com/th-ch/youtube-music
