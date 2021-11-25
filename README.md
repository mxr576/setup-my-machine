## Set up my developer env with Ansible

### Usage

#### First time set up

Install Ansible (latest) from the official PPA:

```sh
$ sudo apt install software-properties-common
$ sudo add-apt-repository --yes ppa:ansible/ansible
$ sudo apt update
$ sudo apt install ansible
```

Make sure the root user has a password, required for `become`:

```
$ sudo su root
$ passwd
```

Copy `example.hosts.yml` to `hosts.yml` and customize it.

### Install dependencies and run the playbook

```
$ ansible-galaxy install -r requirements.yml  --ignore-errors
$ ansible-playbook playbook.yml --ask-become-pass
```

System restart could be required, at least after the first run.

### Tested on

* Linuxmint Cinnamon 20.2/Ubuntu 20.4
* Ansible 2.11.6
