Ansible roles to manage OpenVPN IPv6-tunnel broker
==================================================

This repository contains (incomplete) ansible playbook to
deploy IPv6 tunnel broker (`site.yaml`) as well as to manage
users' tunnels (`certs.yaml`). Client database is stored in
`clientlist.yaml` file with a structure like this:


        ---
        
        ipv6tun_clients:
          - id: 210
            client: user1
            email: some@email.example
          - id: 211
            client: user2
            email: some@email.example
            ticket: 123456
        
        ...
