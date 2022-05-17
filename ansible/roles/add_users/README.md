# Add Users

add users with their ssh_keys into the hosts

## Requirements

no requirements needed.

## Role Variables

- **users:** dictionary of users and their public_key to add in the host(s)

  - Users MUST have 2 keys:
    - username
    - ssh_key

- **sshd_config:** path of the sshd_config in the host(s)

## Other default vars:

- ansible_ssh_port
- ansible_user
