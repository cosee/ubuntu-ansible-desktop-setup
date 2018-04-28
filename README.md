# Install Ansible
Execute the `install.sh` and follow the instructions.

# Applications
You can modify the `setup.yml` to use install only applications you need.

After installing ansible via the `install.sh` you can execute the playbook with:

`ansible-playbook setup.yml --ask-become-pass`

By default it installs the following:

Java 8

Chrome

htop

gitk

xclip

Hamster Time Tracker (TODO not available in apt repository)