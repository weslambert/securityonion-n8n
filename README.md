# securityonion-n8n
Install n8n on Security Onion 2.3 to assist with automating context gathering and response.

NOTE: THIS IS ONLY SUPPORTED FOR SECURITY ONION 2.3, AND WILL NOT WORK ON THE LATEST VERSION OF SECURITY ONION

### Overview
This script and the accompanying components will setup n8n on [Security Onion (2)](https://github.com/Security-Onion-Solutions/securityonion).

### Notes
- This is NOT an officially supported Security Onion integration -- please use it at your own risk.
- This script and the accompanying components have only been tested on a standalone node, although it should work fine for a manager, or managersearch node.

### Installation
To get started, clone the repo, then run the `install_n8n` script:

```
git clone https://github.com/weslambert/securityonion-n8n    
cd securityonion-n8n  
sudo ./install_n8n
```
The script will do a few things:

- Pull down `wlambert/n8n` (pre-built n8n Docker image containing [pyvelociraptor](https://github.com/Velocidex/pyvelociraptor))
- Copy Salt/Nginx configuration for n8n
- Restart services as necessary
