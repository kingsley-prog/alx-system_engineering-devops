# Understanding Shell Permissions

## Commands to explore:
    chmod
    sudo
    su
    chown
    chgrp
    id 
    groups
    whoami
    adduser
    useradd
    addgroup

## Objectives:
    to understand what the above commands does and how to use them effectively.
    an understanding of file permissions.


## concepts to explore
    How to create a user
    How to create a group
    how to print real and effective user and group ids
    How to print the effective userid and groups a user in

1. useradd: 
syntax: useradd [options] username
Note: only use with sudo rights can use othe above commands to create new user accounts.
this commands adds the user account created to the /etc/default/useradd file.

__usage__: sudo useradd username

password is required to login- to set passwd for the new user use
sudo passwd username

To Add and create a New user and create a Home Directory:
sudo useradd -m username

Creating a user with specific Home directory( the specify directory is /opt)
sudo useradd -m -d /opt/username username


Creating a user  with specific User Id
sudo useradd -u 1500 username

2. su: switch user or substitute user
su - account
