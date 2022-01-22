# ansible-role-blender

## how to use

Put them in your requirements.yml like this
---
- src: https://github.com/tuanvu0606/ansible-role-blender.git
  name: remote-tuanvu-blender
  version: main
---

then download the repo by this command

```
ansible-galaxy install -r ./playbook/requirements.yml --force
```

Refer to the roles like this:
---
- name: onprem general windows 10
  hosts:     
    onprem-general-windows
  roles:
    - remote-tuanvu-blender
---