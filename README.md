## IAC Ansible
writing iac / declaring infrastructure and then have it built or created. It can create machines


## How it works

## How to set it up
We are setting up our controller machine in AWS. ansible_bash is a script that will install ansible and associated dependencies.

## Main Sections

## Main Commands

## Configuring a server

## Mutable VS Immutable

Mutable- changes and can be changed.
Immutatble - can't be changed.

Largely mostly have used mutable environments, ssh in, run bash, restart servers and get it to the place that the machine needs to be.

Making something from scratch has its drawbacks as it might take longer but in the long run it's more efficient as you get more predictable results.

## Configuration Management

They help configure and test machines to a specific state.
They also help with maintainance of the system
- Puppet
- Chef
- Ansible (Push configuration management)

Packer or ansible --> Create the AMI
They have a controller - agent relationship

They help provision:
- Install packages
- Config Files
- Send in Files
- Environment Variables
- Start and enable services


## Orchestration 
Once we have a machine image, orchestrations tools are used to deploy these into more complex environments. These tools focus on the networking and architectrue rather than the configuration of the individual machines.
They focus more on the environment where these machines run.

- Terraform
- Ansible
- Cloud Formation


## Ansible Intro
Configuration management software
Allows you to make changes to machines in a declarative way through a "push" system

## Platform Agnostic - Less Vendor locking
With the ansible abstraction layer you can run the code in any environment for any OS and it will know how to install and perform the operation

Example:
- Ubuntu uses : apt and apt-get
- Centos : dnf or yum
- IOS : brew and others

## Testing Strategies 