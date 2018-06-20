# Install Ansible
Execute the `install.sh` and follow the instructions.

# Applications
You must modify the `setup.yml` to install only applications you want. By default all applications and configurations are commented out.

To include applications just uncomment the packages.

After installing ansible via the `install.sh` you can execute the playbook with:

`ansible-playbook setup.yml --ask-become-pass`

Look into the `defaults.yml` and change variables as you need. E.g. you will need to change 'docker_user' to your username in order for ansible to configure the docker group correctly.

You will have to logout/login for all changes to take affect (docker).

## By default following applications are available:

- Java 8

- Chrome

- Slack

- Docker (latest)

- Docker-compose (1.21.0, set different version in defaults.yml)

- Maven

- IntelliJ

- Postman

- Tilix (Terminal)

- Sublime-Text 3

- Fish (instead of Bash)

- Oh my fish (with theme BobTheFish for fish)

- NodeJS (version 9.x, change version in the defaults)

- Angular-CLI

- openvpn

- gimp

- spotify

- pip

- pytest

- htop

- gitk

- xclip

(- Hamster Time Tracker (TODO not available in apt repository))

## Default configurations:

- Disable Mouse acceleration (only for mice, not touchpad)

- Remove Amazon app

## KDE only

- Set meta only shortcut to present window overview
