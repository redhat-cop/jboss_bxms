Ansible JBoss BxMS Role  [![Build Status](https://travis-ci.org/redhat-cop/jboss_bxms.svg)](https://travis-ci.org/redhat-cop/jboss_bxms)
=================

A role to install JBoss BRMS or BPM Suite on RHEL6 and 7. Intended to be used with [JBoss Middleware Playbooks](https://github.com/redhat-cop/ansible-middleware-playbooks)

Transfer Method
------------

This role supports a few different mechanism for transferring the product zip files to the target host. These are documented on [the main playbooks README](https://github.com/redhat-cop/ansible-middleware-playbooks), as the methods are supported across a variety of roles.

Dependencies
------------

- java
- unzip

Our playbooks provide these dependencies in a [common role](https://github.com/redhat-cop/ansible-middleware-playbooks/tree/master/roles/common), but this there is no explicitly ansible dependency to allow end users more options.

Default User
------------

A default user can be created for you by setting the variable `jboss_bxms_create_default_eap_user == true`. This will create user `jboss` with password `bpmsuite1!`. This only works for EAP for now. You can see the roles defined [here](files/application-roles.properties).

License
-------

[LICENSE](./LICENSE)

Authors Information
------------------

* [Andrew Block](https://github.com/sabre1041)
* [Justin Holmes](https://github.com/sherl0cks)
* [Kamesh Sampath](https://github.com/kameshsampath)
