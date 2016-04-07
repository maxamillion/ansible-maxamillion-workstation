# ansible-maxamillion-workstation

Adam Miller (maxamillion) ansible playbook for Fedora workstation/laptop setup
and configuration

## Usage

Install [Fedora Server](https://getfedora.org/en/server/)

Install `ansible` and `git`

    dnf -y install ansible git

Clone this repo and run the ansible-playbook (run the `bootstrap-fedora` if
running Fedora 23 or later).

    git clone https://github.com/maxamillion/ansible-maxamillion-workstation.git
    cd ansible-maxamillion-workstation
    ansible-playbook bootstrap-fedora.yml -i inventory.txt
    ansible-playbook workstation.yml -i inventory.txt

### Notes
There are no dotfiles or configs included in this ansible-playbook.
Data retention is handled outside the scope of this playbook

Some of my dotfiles related to i3, i3status, dunst, and tmux are available [here](https://github.com/maxamillion/dotfiles).

### References
[Ansible](http://www.ansible.com/home)
[Ansible Docs](http://docs.ansible.com/ansible/index.html)
