Playbook description
=========

Initial setup and configuration of a freshly installed Raspberry Pi OS

Playbook will do initial patching, setup a new sudo user/replace the default pi user, copy authorized ssh keys (from the system running the playbook), setup wifi and harden its ssh_config file

1. Clone this repo down
2. cd into the the cloned directory
3. run ```ansible-galaxy role install -r roles/requirements.yml``` to install all required ansible roles
4. update the ```inventory``` file with the ip or hostname of your newly provisioned raspberry pi
5. run ```ansible-playbook main.yml -K --user pi -i inventory``` to start the setup of raspberry pi
6. Follow the prompts for setting up your new user and wifi.


License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
