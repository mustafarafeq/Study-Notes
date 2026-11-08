# This Document is for documenting Common Linux Commands and their uses. 

| RHEL Command	| Regular Linux (Ubuntu/Debian) Command	| What it does |
| --- | --- | --- |
| dnf install nginx	| apt install nginx | Install software |
| dnf update | apt update && apt upgrade | Update packages |
| rpm -qa | dpkg -l	| List installed packages |
| systemctl status sshd | systemctl status ssh | Check SSH service |
| sestatus | aa-status | Check security framework (SELinux/AppArmor) |
| firewall-cmd --list-all | ufw status | Check firewall rules |
| nmcli | netplan | Network configuration tools |
| fips-mode-setup --check |	No direct equivalent | Check RHEL FIPS mode |
| ip addr |	ip addr | Show IP addresses |
| ip route | ip route | Show routing table |
| df -h | df -h	| Show disk usage |
| du -sh /var |	du -sh /var | Show directory size |
| lsblk | lsblk	| List disks |
| mount | mount | Show mounted filesystems |
| showmount -e server |	showmount -e server | Show NFS exports |
| ps aux |	ps aux | List processes |
| top | top | Monitor processes |
| free -h |	free -h | Show memory usage |
| journalctl -xe | journalctl -xe | Review system logs |
| ausearch -m AVC |	ausearch -m AVC* | Search audit events |
| auditctl -l |	auditctl -l* | List audit rules |
| tar -czvf | tar -czvf | Create compressed archive |
| gzip file | gzip file	| Compress file |
| unzip file.zip | unzip file.zip | Extract ZIP archive |
| scp file user@host:/path | scp file user@host:/path | Transfer files securely |
| openssl s_client | openssl s_client | Inspect TLS connection |
| sar -u 1 5 | sar -u 1 5 | Monitor CPU activity |
| truncate -s 0 file.log | truncate -s 0 file.log | Empties a file while preserving the file itself, its                                                            ownership, and permissions. |