# How to Create a VPN Tunnel

## Prerequisites

- A VPS (Virtual Private Server) from any provider (e.g., [DigitalOcean Droplet](https://m.do.co/c/2e751e58353f))
- A domain setup with [DuckDNS](https://www.duckdns.org/) or any other dynamic DNS service

## Steps

### 1. Purchase and Setup VPS

Purchase a VPS from any provider. I recommend using a [DigitalOcean Droplet](https://m.do.co/c/2e751e58353f).

### 2. Log in to Your Server

Connect to your VPS via SSH:

```bash
ssh root@your-server-ip

```

### 3. Update and Upgrade Packages

Run the following commands to update your system:

```bash
sudo apt-get update && sudo apt-get upgrade -y

```

### 4. Clone the Repository

Navigate to the temporary directory and clone the repository:

```bash
cd /tmp
git clone https://github.com/isharax9/3x-ui-mod.git
cd 3x-ui-mod

```

### 5. Install the Application

Start the installation process:

```bash
bash install.sh

```

When prompted, set up your panel credentials.

### 6. Install Certbot

Install Certbot for SSL certificate management:

```bash
sudo apt-get install certbot -y

```

### 7. Create and Configure Domain

Set up a domain through [DuckDNS](https://www.duckdns.org/) and point it to your server's IP address.

### 8. Generate SSL Certificates

Create SSL certificates for your domain:

```bash
sudo certbot certonly --standalone --agree-tos --register-unsafely-without-email -d your-domain.duckdns.org

```

Store the generated PEM keys in a secure location. 🔐

### 9. Enable Port Access

Open the required ports (80 and 443 for HTTP/HTTPS) in your server provider's dashboard.

## Conclusion

Your VPN tunnel is now ready to use. Access the control panel through your domain.

---

Feel free to customize this further to suit your needs!

---
## Client tools for connecting to the VPN

### 1. V2rayN - https://github.com/2dust/v2rayN (recommended☑️) 
### 2. Netch - https://github.com/netchx/netch

