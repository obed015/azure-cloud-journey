# VM Troubleshooting Scenarios

## Scenario 1: SSH Timeout
- Cause: Missing NSG rule, UFW blocking, SSH service down
- Fix: Serial Console + ufw allow ssh + restart sshd

## Scenario 2: No Internet
- Cause: No public IP, DNS misconfigured
- Fix: Assign Static IP, check /etc/resolv.conf, ping 8.8.8.8

## Scenario 3: Disk Not Visible
- Fix:
  1. lsblk
  2. fdisk
  3. mkfs.ext4
  4. mount + fstab

## Scenario 4: VM Won’t Boot
- Use Boot Diagnostics + Serial Console
- If needed: detach disk → attach to healthy VM → mount

## Scenario 5: NSG Deleted
- Fix: Re-attach NSG to NIC via portal or CLI
- OR: Use Serial Console to open UFW temporarily
