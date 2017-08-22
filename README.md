rhn_subscription
=========

This role is used for subscribing machines to the Red Hat Network.

Requirements
------------

Red Hat account with the appropriate entitlements for desired red hat products

Role Variables
--------------
| variable                 | required | default | choices | comments                                            |
|--------------------------|----------|---------|---------|-----------------------------------------------------|
| rhn_user               | yes        | undefined        |         | User account to use for RHN  |
| rhn_password           | yes        | undefined        |         | User password to use for RHN |
| rhn_product            | yes        | undefined        |         | Product name to search for |
| rhn_subscription_clean | no         | false   | true/false        | Use this if you want to clean out all existing subscriptions on each run |
| rhn_pool_id            | no         | undefined |         | Define if you want to use a static Pool Id instead of searching for available pools |

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
