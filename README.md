Ansible Role: Hello World
=========

An Hello World, Ansible role for testing purposes


Requirements
------------

None.

Role Variables
--------------

See the `defaults/main.yml`.

```
world: "world"
```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: helloworld }

Execute result:

	$ ansible-playbook setup.yml
	
	PLAY [Play 'Hello World'] ******************************************************
	
	TASK [setup] *******************************************************************
	ok: [localhost]
	
	TASK [echo 'hello world'] ******************************************************
	changed: [localhost]
	
	TASK [print message] ***********************************************************
	ok: [localhost] => {
	    "msg": [
	        "Hello world"
	    ]
	}
	
	PLAY RECAP *********************************************************************
	localhost                  : ok=3    changed=1    unreachable=0    failed=0


