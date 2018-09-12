zabbix-agent-win
=========

Configures zabbix agent for windows using chocolatey packages

Requirements
------------

dnspython module for the ansible controller.
install with "pip install dnspython"

Role Variables
--------------
zabbix_server: dns name of zabbix server. Inherited from global scope.

zbx_agent_configpath: used to specify the zabbix_agentd.conf file location.
zbx_agent_logpath: used to specify the zabbix_agent.log file location.
zabbix_server_ip: uses the dig lookup to get the ip of zabbix_server for creating firewall rules.

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: windows_servers
      roles:
         - { role: zabbix-agent-win, zabbix_server: zabbix }

License
-------

GPLv3

Author Information
------------------

Jeff Hibberd
