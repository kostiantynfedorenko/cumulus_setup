# Configuring Cumulus VX

This Ansible playbook configures 4 VMs in leaf-spine topology.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine.

### Prerequisites

I suggest using python VENV to work with this playbook.
Instructions on how to create a virtual environment can be found here - [VIRTUALENV](https://virtualenv.pypa.io/en/stable/).

### Installing

I use VirtualBox environment to run 4 cumulus VX devices.
HOWTO for VirtualBox and Cumulus - [VirtualBox&Cumulus](https://docs.cumulusnetworks.com/display/VX/VirtualBox).
Two-leaf&Two-spine topology - [TwoLeaf&TwoSpine](https://docs.cumulusnetworks.com/display/VX/Create+a+Two-Leaf%2C+Two-Spine+Topology).

## Running

Use the following command to run the playbook:
```
ansible-playbook site.yml -i inventories/hosts --ask-become-pass
```
Do not hesitate to use options like:
```
-C, --check           don't make any changes; instead, try to predict some
                      of the changes that may occur
-D, --diff            when changing (small) files and templates, show the
                      differences in those files; works great with --check
--step                one-step-at-a-time: confirm each task before running
-v, --verbose         verbose mode (-vvv for more, -vvvv to enable connection debugging)
```
