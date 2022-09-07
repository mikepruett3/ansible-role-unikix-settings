Ansible Role: NTT Data UniKix Server Settings
=========

Ansible role to configure NTT Data UniKix Server settings on Linux Servers.

Requirements
------------

The role does not require anything to run on Ubuntu, Debian or RHEL and its derivatives.

Role Variables
--------------

Available variables are listed below, along with default values (see ```defaults/main.yml```):

``` yaml
proxy_host: "myproxyserver.example.com"
```

```proxy_host:``` **(Required)** Hostname or IP Address of the Proxy Server to use.

```proxy_port:``` **(Required)** Port to use to connect with the Proxy Server.

```proxy_protocol``` **(Required)** Protocol to use to connect with the Proxy Server. This should be either **http** or **https**.

Role variables can be stored with the ```hosts.yaml``` file, or in the main variables file.

Dependencies
------------

None.

Example Playbook
----------------

``` yaml
    - hosts: servers
      roles:
         - role: mikepruett3.apache-settings
```

License
-------

MIT

Author Information
------------------

Role created by [mikepruett3](https://github.com/mikepruett3) on [Github.com](https://github.com/mikepruett3/ansible-role-apache-settings)
