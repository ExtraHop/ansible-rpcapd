Role Name
=========

rpcapd role automates the installation of rpcapd on Linux systems.

Requirements
------------

No other roles are required.

Role Variables
--------------

- extrahop_rpcapd_target = *unset*
  No default. Set this to the IP or hostname
  of the ExtraHop EDA you want the system to forward packets to.

- extrahop_rpcapd_port = 2003 (Default)

- extrahop_rpcapd_second_target = *unset*
  No default. Set this to the IP or hostname
  of the 2nd ExtraHop EDA you want the system to forward packets to.
  Rarely used.

- extrahop_rpcapd_interface = *unset*
  No default. Set this to the interface name i.e. eth0 of the sender.
  If, and only if, a 2nd rpcapd target is defined, this variable
  is required.

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: extrahop.rpcapd, : extrahop_rpcapd_target = foo.example.com }

License
-------

BSD


