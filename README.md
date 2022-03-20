# Wiki.js Automation

This playbook is based on [Wiki.js installation guide](https://docs.requarks.io/install/ubuntu).

To install Wiki.js on a new Ubuntu server:

1. Update target server IP: `inventory/production`
1. Update A record for the new wiki domain name.
1. Run the playbook: `./provision.sh`
1. Open `http://your-server-ip` in browser to complete the on-screen setup.
1. Make sure to replace email and domain name with actual values, and run the second playbook: `LETSENCRYPT_DOMAIN=wiki.example.com LETSENCRYPT_EMAIL=admin@example.com ./enable_https.sh`
1. [Redirect HTTP requests to HTTPS](https://docs.requarks.io/install/ubuntu).
