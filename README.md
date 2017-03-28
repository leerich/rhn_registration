rhn_subscription
=========

Basic role that does not utilize the subscription-manager module (significantly slower at large scale)

Requirements
------------

Red Hat account with the appropriate entitlements for desired red hat products

Role Variables
--------------

rhn_user
- The user account you want to use when registering to RHN

rhn_password
- Password you would like to use. I'd recommend stashing this in a vault file.

rhn_product
- The product you would like to register (i.e. OpenShift, Satellite, Red Hat Enterprise Linux, etc)

Dependencies
------------

No dependencies

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: josh-springer.rhn_registration, rhn_user: foo }

License
-------

BSD

Author Information
------------------

Josh Springer
