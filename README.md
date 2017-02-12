VPC
===

Creates a VPC inside AWS including any defined dependencies (subnets, security groups, network ACLs etc)

Requirements
------------

boto, boto3 libraries

Role Variables
--------------

* `vpc_cidr` - CIDR for the VPC
* `vpc_tags` - tags to apply to the VPC
* `vpc_subnets` - a list of subnet dicts. Each subnet should include the following keys: `az`, `cidr`, `name`, `tags`
* `vpc_security_groups` - a list of security groups.
* `vpc_network_acls` - a list of network ACLs



Dependencies
------------



Example Playbook
----------------

- hosts: production
  connection: localhost
 
  roles: 
  - vpc

License
-------

BSD

Author Information
------------------

Will Thames <will@thames.id.au>
