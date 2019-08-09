# defaultjson_ansible_callback
* Extends Ansible default STDOUT callback to write json log file if ANSIBLE_JSON_LOG_FILE is set. Default output will still go to STDOUT
* This is simply a merge of default.py and json.py from https://github.com/ansible/ansible/tree/devel/lib/ansible/plugins/callback


# usage:
For single play usage, copy into callback_plugins folder relative to playbook and export environment variable
```bash
export ANSIBLE_STDOUT_CALLBACK=defaultjson
export ANSIBLE_JSON_LOG_FILE=test.log
```

# debug:
To send JSON dump to STDOUT, export ANSIBLE_JSON_LOG_DEBUG
e.g.
```bash
export ANSIBLE_JSON_LOG_DEBUG=true
```





