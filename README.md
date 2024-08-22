# ansible
My ansible scripts for my home server project using raspberry pi's

INFO:
Rasberry pi 5: Amount 2



Commands Used:
ansible all -m ping -> Makes contact with all host making sure they are acessible
ansible all -m gather_facts -> Gathers facts on all my host
ansible all -m apt -a name=neovim --become --ask-become-pass -> Installs neovim on all my hosts
