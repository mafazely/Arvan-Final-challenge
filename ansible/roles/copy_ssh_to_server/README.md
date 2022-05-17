# Role Name

A role for adding public keys specified to target servers specified, used mainly for database authorization to gateway servers.

## Requirements

- existing public keys on master node

## Summary

This role will loop on targeted server group for example `databases` and add public keys generated for example `fetched/id_rsa_db1.pub` to the target servers.
