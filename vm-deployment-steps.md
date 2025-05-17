# VM Deployment (Linux & Windows)

## Ubuntu VM (Zone 1)
- VM Name: WebVM1
- Zone: 1
- Public IP: Dynamic
- Port: 22 allowed via NSG
- NGINX installed

## Windows VM (Zone 2)
- VM Name: WebVM2
- Zone: 2
- Port: 3389 (RDP) allowed
- IIS installed (optional)

## Key Notes:
- VMs are in the same VNet and Subnet (WebSubnet)
- Tested connectivity via internal ping
