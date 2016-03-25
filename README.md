#Ansible Create Sudo User Role
The purpose of creating this role was to assist with creating a user for Chef Client nodes for use with a playbook to bootstrap a Chef Client.

This turns out to be a very common use case, creating a user with sudo privilleges, so it has been generalized and can be used as follows

## Variable Definitions
  - **user**: The name of the user to create (Default: chef)
  - **group**: The home group of the user (Default: chef)
  - **key_dir**: Directory for public key local fs
  - **pubkey_file**: File name for pubkey, if defined, will set up SSH authorized\_keys file
  - **home_dir**: If using a custom home dir, one could override this variable (Default: /home)

## License
This role is licensed under the MIT License, for more details, please view the LICENSE file in the source repository :)
