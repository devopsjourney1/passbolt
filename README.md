# Passbolt Tutorial
## Full Video Tutorial
[See the full YouTube tutorial here](https://youtu.be/O76Lye5D-n8)
  
## Setup
  
  - Modify the .env file with the details of your configuration
  - Create a Cloud Flare Tunnel (Explained below) OR comment out the cloudflare service in the docker-compose file
  - Use docker compose to bring up the services!
  
  ```
  docker compose up
  ```
  
  
## CloudFlare Tunnel setup

1. CloudFlare -> Zero Trust -> Accesss -> Tunnels
  
2. Click: Create a Tunnel
  
3. Name your Tunnel: Give the tunnel a name -> Next
  
4. Install Connector: Copy the key provided to the .env file `CLOUDFLARE_TUNNEL_TOKEN` -> Next
  
5. Fill in domain/subdomain and for Type: http://passbolt:80  -> Done
