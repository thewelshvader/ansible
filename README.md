# ansible

## Find mount point
After outage or upgrades, the primary longhorn node may change. Find out which node is now primary from the longhorn ui and connect over ssh.
Then find the correct mount point using lsblk and update the path in the playbook here **playbooks/music-mgmt.yaml**
```
lsblk -f
```