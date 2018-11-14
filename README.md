# Install Ansible
Execute the `install.sh` and follow the instructions.

The `install-git-and-ansible.sh` file is available for independent installation via e.g. USB. It installs git + ansible and pulls the project so everything is ready to go.

# Applications
You must modify the `setup.yml` to install only applications you want. By default all applications and configurations are commented out.

To include applications just uncomment the packages.

After installing ansible via the `install.sh` you can execute the playbook with:

`ansible-playbook setup.yml --ask-become-pass`

Remote setup is only possible if the server has the ssh daemon installed.

Look into the `defaults.yml` and change variables as you need. E.g. you will need to change 'docker_user' to your username in order for ansible to configure the docker group correctly.

You will have to logout/login for all changes to take affect (docker).

## By default following applications are available:

- Java 8

- Chrome

- Slack

- Docker (latest)

- Docker-compose (1.23.1, set different version in defaults.yml)

- Maven

- IntelliJ

- Android-Studio

- Postman

- Tilix (Terminal)

- Sublime-Text 3

- notepadqq

- Atom

- GHex

- Fish (instead of Bash)

- Oh my fish (with theme BobTheFish for fish)

- NodeJS (version 9.x, change version in the defaults)

- Angular-CLI

- openvpn

- gimp

- Spotify

- VLC

- pip

- pytest

- aws-cli

- htop

- gitk

- xclip

- Network manager openvpn for Gnome

## Default configurations:

- Increase max number of files to watch for nodejs file watcher (necessary for bigger node_modules directories in projects)

- Disable Mouse acceleration (only for mice, not touchpad)

- Remove Amazon app

## KDE only

- Set meta only shortcut to present window overview
