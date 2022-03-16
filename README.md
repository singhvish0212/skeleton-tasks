# Ansible role: {{ role_name }}

## Description

{{ role_name }} is an Ansible role used to...

## Supported OS

* RedHat
* CentOS

## Requirements

n/a

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    ---
    # defaults file for {{ role_name }}

    # Use '{{ role_name }}_' prefix for all variables

    # Include debug information
    {{ role_name }}_debug: false


## Dependencies

This role uses `other` role.

## Example Playbook


    - name: Play 1
      hosts: all
      gather_facts: true
      become: true

      tasks:
	  
      - import_role:
          name: {{ role_name }}
        vars:
          {{ role_name }}_debug: false
        tags:
          - {{ role_name }}
		  
		  
Inside `vars/main.yml` or `group_vars/..` or `host_vars/..`:


    #-------------------------------------------------
    # overrides role '{{ role_name }}' variables
    #-------------------------------------------------

    {{ role_name }}_debug: true
	
    # ... etc ...
	
	
## License

GPLv3 - GNU General Public License v3.0
� Automation OOGH

## Authors

- [Finashu](mailto:finashu.f@hcl.com)

## Reviewer

- [Mohit Yadav](mailto:mohit-yadav@hcl.com)


