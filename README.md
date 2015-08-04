# sentinel
Installs XWiki on LXC containers using Ansible

This playbook uses lxc_container which is only available on version 1.8 and above of ansible.
Please ensure you have added the ansible repository and installed the latest version of ansible
before attaempting to run this playbook:

apt-add-repository ppa:ansible/ansible
apt-get update
apt-get install ansible

ansible-playbook --verbose xwiki.yml

Note: Playbook assumes a user account named sshafiullah is present on the target server
      and has sudo privileges. Change this user at the top of the xwiki.yml file

Note: Adjust the /etc/ansible/hosts and replace 'localhost' with a target server
