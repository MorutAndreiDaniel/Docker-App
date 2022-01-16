# Docker-App
This is a simple Docker App deployed using Ansible.
The repository contains a directory with a video of the running App, on a local VirtualBox server. Also, it contains 2 directories (spec and src) with app's code.
And the last directory contains the templates for every step of the playbook.
In the root directory, is the Dockerfile which is used for building the image of the app. An ansible.cfg, in which is stored the values for inventory file name and
path of ssh keys for connecting to remote server.
Also in the root directory, are stored the inventory (with host name value and variables) and the playbook that is used by Ansible to build and deploy the container 
for app on remote servers, which is called install_docker_app.yml and can be run with command: "ansible-playbook install_docker_app.yml --ask-become"
