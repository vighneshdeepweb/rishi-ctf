# Radio Active

```bash
Machine Name : "Radio Active"
Machine Difficulty : "Easy"
Oprating System : "CentOS Server or Linux"
```

## Starting 

### Ports

```perl
8910 - SSH
9001 - FTP
```

### FTP 
We will Allow Anonymous FTP Login so people can login and get rsa key

### Rabbit Hole
We will put corrupted RSA key of SSH of  user but the rsa key with encryption and when you'll able to crack to the hash you'll get password of ssh

```
Cracking Method :- ippsec's Delivery Root Hash Cracking
```
## Priv Esc 

```perl
After Login user can run a python file in /tmp.

Because everyone can open /tmp.
```

```php
sudo -l

The Out must be the user can access /tmp/something.py with sudo
```
### On the /tmp
```bash
#user@host:~ ls
.
..
something.py 
```

which is editable with "vi editor" as a user so players can edit and put any python reverse shell from websites like high on coffee or pen test monkey 

```bash
nc -lvnp 8888
root@hostname:~whoami
root
```
