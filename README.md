# ansible
My ansible scripts for my home server project using raspberry pi's

INFO:
Rasberry pi 5: So far I have 2 rasbery pi nodes running rasberry pi OS lite
Master Node: I am running ansible through my alma linux wsl machine


Steps:
- Made sure that I could contact all my nodes through ssh using a dedicated ansible key only for ansible, reasing being is that ansible uses ssh to manage nodes \
- Made plays that installed and removed apache2 from all nodes



Commands Used:
ansible all -m ping -> Makes contact with all host making sure they are acessible \
ansible all -m gather_facts -> Gathers facts on all my host \
ansible all -m apt -a name=neovim --become --ask-become-pass -> Installs neovim on all my hosts
