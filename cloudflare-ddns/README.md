Role Name
========

This role deploys a docker container on your raspberry-pi to update your Cloudflares A-Record with your current public IP-Address

Requirements
------------

To run this role you will need to fullfill the following requirements:

- a domain (can be bought anywhere)
- a cloudflare.com account
- a cloudflare API-Key
- your cloudflare account has to be connected with your domain providers account (change nameserver to the ones provided by cloudflare white setting up your site)
- a raspberry-pi (can be anyone)
- the pi needs to be connected to the internet
- docker on your raspberry-pi

Role Variables
--------------

To run this role you will need to edit the file ```vars/main.yml``` and change the two following variables.

```
---
cloudflare_api_key: "GENERATED_CLOUDFLARE_API_KEY_HERE"     # <- enter your API-key here
domain: "YOUR_DOMAIN_HERE"                                  # <- enter your domain here (no subdomains f.e. examle.com )
``` 

Dependencies
------------

ROLE TO DEPLOY DOCKER FOR PI HERE LINKED
A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - cloudflare-ddns

    
License
-------

BSD

Author Information
------------------

Name: Stiven Stepanovic
GitHub: https://github.com/Styvven
Contact: 
