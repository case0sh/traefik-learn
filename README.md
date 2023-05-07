# Basic configuration of Traefik

This example shows a basic configuration of Traefik with a secure connection. 

## Getting Started

### Prerequisites

1. A domain name, we assume for this example the domain `example.com` (access from internet and SSL certificate).
2. Cloudflare's account
3. A working installation of `docker` and `docker-compose`
4. Port 80 and 443 are not used.


### Installing

1. All the configurations are in the `docker-compose.yml` file.

2. Copy from the root folder the `var.env` file and rename it in `.env`.

3. Change all the needed variables with the values of your case. The following list shows the needed for traefik and whoami test container:

```yml
DOMAIN              #domain name
CLOUDFLARE_EMAIL    #Cloudflare email account
CLOUDFLARE_API_KEY  #Cloudflare API key
ACME_EMAIL          #Reminder email for the generated certificate
```
