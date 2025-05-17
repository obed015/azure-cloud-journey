# Azure Storage Notes

## Types of Storage
- Blob (Unstructured files)
- File (SMB-based sharing between VMs)
- Queue (Message passing)
- Table (NoSQL)

## What I did:
- Created a Storage Account (LRS, Hot tier)
- Created and mounted a File Share
- Attached a 4GB Data Disk and mounted on Ubuntu VM using:
  - fdisk
  - mkfs.ext4
  - /etc/fstab
