# vagrantctl

A simple tool that utilizes Vagrant and enables you to keep track of multiple different Vagrant environments in the same repository.

## Why?

I use this mainly for testing Ansible roles that are held in the same repository.

## Installation

Clone this repository/Copy these files to the root of your repository.

## Usage

```
./vagrantctl.sh <option> <environment> [vm (optional)]

up [vm]           - Starts the VMs in the environment (vagrant up).
halt [vm]         - Stops the VMs in the environment (vagrant halt).
init              - Initializes the environment.
status [vm]       - Shows the status of the VMs in the environment.
global-status     - Same as vagrant global-status.
destroy [vm]      - Destroys the VMs in the environment. NOTE: Does not destroy the env directory.
complete-destroy  - Destroys the whole environment (VMs AND directory). Use carefully.
help              - Prints this usage message.
list              - List all environments.
ssh <vm>          - Opens up an SSH connection to a VM.
```
