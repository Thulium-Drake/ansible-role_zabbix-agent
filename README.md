# Zabbix agent as configured by Ansible
This role can configure an Zabbix agent on your Ansible managed hosts.

It will install an agent and configure it for use with a Zabbix server using
PSK encrypted connections. The keys required for the connection are generated
using a deterministic approach, so they don't have to be saved on the ansible
controller.

This role is also able to deploy supporting scripts for Zabbix templates such as
the ones in https://github.com/Thulium-Drake/zabbix-templates.

If you have your own collection of Zabbix templates, you can still use this role if
you place your template scripts and configs in a similar structure.

## Setup
Incorporate the role in your regular Ansible playbooks and configure it.