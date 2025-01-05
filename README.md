# How to make a VPN Tunnel for your convenience
First Buy a VPS from any where, but i am recommending is Digital Ocean Droplet 💧 

log in to the server and execute below commands 

`sudo bash`

`apt-get update && apt-get upgrade -y`

`cd /tmp`

`git clone https://github.com/isharax9/3x-ui-mod.git`

`cd 3x-ui-mod`

`bash install.sh`

add panel credentials and save them

`apt-get install certbot -y`

create a domain from duckDNS to your server ip

`certbot certonly --standalone --agree-tos --register-unsafely-without-email -d your-domain.duckdns.org`

copy those pem keys and store them 🗝

open port access on server provider dashboard
