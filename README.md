Ansible Role: splatnet2statink container
=========

Build [splatnet2statink](https://github.com/frozenpandaman/splatnet2statink) container for podman environment.

Requirements
------------

This requires podman installed on target system.

Role Variables
--------------

|Name|Comment|
|----|----|
|splatnet2statink_version|Version of splatnet2statink.|
|splatnet2statink_config||List of splatnet2statink config. Parameter details are below. (Default: [])|

|Parameter|Comment|
|----|----|
|name|Name of config. *Required*|
|api_key|API key for stat.ink|
|cookie|Cookie for accessing nintendo|
|session_token|Token for accessing nintendo|
|user_lang|Language of stat.ink|
|salmon|Get salmon run data. (Default: `no`)|
|timer_delay|Checking for new results every this configuration. (Default: `5min`)|

Dependencies
------------

None.

Example Playbook
----------------

```
- hosts: localhost
  roles:
   - grahamoon.splatnet2statink-container
```

License
-------

Apache

Author Information
------------------

Grahamoon

