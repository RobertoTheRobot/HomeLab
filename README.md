# HomeLab
This repo contains configuration files to run a home lab.

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


### Links:
- Install haproxy + using OpenSSL: 
https://www.upcloud.com/support/haproxy-load-balancer-centos/#installing-haproxy
http://virtuallyhyper.com/2013/05/configure-haproxy-to-load-balance-sites-with-ssl/
https://seanmcgary.com/posts/using-sslhttps-with-haproxy/

- Install certbot for haproxy: 
https://certbot.eff.org/#centosrhel7-haproxy

- SSL termination haproxy + autorenewal: 
https://www.digitalocean.com/community/tutorials/how-to-implement-ssl-termination-with-haproxy-on-ubuntu-14-04
https://www.digitalocean.com/community/tutorials/how-to-secure-haproxy-with-let-s-encrypt-on-ubuntu-14-04

