# Install Ansible
Execute the `install.sh` and follow the instructions.

# Applications
You can modify the `setup.yml` to use install only applications you need.

After installing ansible via the `install.sh` you can execute the playbook with:

`ansible-playbook setup.yml --ask-become-pass`

Look into the `defaults.yml` and change variables as you need. E.g. you will need to change 'docker_user' to your username in order for ansible to configure the docker group correctly.

You will have to logout/login for all changes to take affect (docker).

## By default it installs the following:

- Java 8

- Chrome

- Slack

- Docker (latest)

- Docker-compose (1.21.0, set different version in defaults.yml)

- htop

- gitk

- xclip

(- Hamster Time Tracker (TODO not available in apt repository))

## Default configurations:

- Disable Mouse acceleration (only for mice, not touchpad)

- Remove Amazon app
