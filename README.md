# Ansible Kontena Agent

<br />

<p align="center">
    <a href="https://kontena.io/">
        <img src="https://kontena.io/images/kontena-logo.svg" width="280">
    </a>
</p>

<br />
<br />

[![Build Status](https://travis-ci.org/roquie/ansible-kontena-agent.svg?branch=master)](https://travis-ci.org/roquie/ansible-kontena-agent)

Ansible role to install Kontena Agent on Nodes.

Example, how to use, can be found at `tests` directory.


## Install

```
ansible-galaxy install roquie.ansible-kontena-agent
```

## Important

Kontena-agent package does not require NTP for installation, but it is strongly recommended by kontena's documentation, 
so you should supply NTP on your hosts by self. We advise to use these role:
[galexrt.ansible-ntpdate](https://github.com/galexrt/ansible-ntpdate).

## Supported OS

For now supports:
* Ubuntu 16.04 LTS
* Ubuntu 14.04 LTS

## Vagrant

* `cd /path/to/project`
* `cd tests && ansible-galaxy install -r requirements.yml && cd ..`
* `vagrant up` 

### Warning
If u want rename project, make sure to rename role (`ansible-kontena-agent`) in `tests/playbooks/vagrant.yml` file.

## License

MIT
