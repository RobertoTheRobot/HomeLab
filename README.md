# HomeLab
This repo contains configuration files to run a hom lab.

## Infrastructure
### VMWare ESXi running virtual machines
- lb-01: haproxy
- es-node-01: elasticsearch node
- appweb-01: Web application server running Kibana and other .net core applications
### Synology ds216
Used to host files and run DDNS job

## DHCP
DHCP provided by TP Link Archer C5
All VMs have a DHCP reservation

## DNS
- Dynamic DNS from default Synology application: http://www.noip.com/support/knowledgebase/enable-ddns-within-synology-device/
- FreeDNS as DNS provider: http://freedns.afraid.org/

## Security
- Certificate Authority: https://letsencrypt.org/
- Managed with https://certbot.eff.org
