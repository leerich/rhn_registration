rhn_subscription
=========

This role is used for subscribing machines to the Red Hat Network.

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
