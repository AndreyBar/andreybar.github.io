# How to extend EBS volume for EC2 instance

## Extend an EBS volume
1. Go to EC2 -> EBS
2. Click desired volume
3. Edit its size
4. Done.

## Extend volume size in EC2

```bash 
df -h
lsblk
sudo growpart /dev/xvda 1
sudo xfs_growfs /dev/xvda1
```