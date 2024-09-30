# Tortoise

This project contains the definition for a Vagrant environment that I use 
instead of my physical host for doing sketchy things on the internet.

This project also serves as an introduction to Linux (more specifically Fedora)
hardening practices.

## Usage

Set your variables in `credentials.yml` (Ansible will read this when Vagrant 
runs provisioning):

```
---

root_password: <root_password>
password: <password>
username: <username>
```

then

`vagrant up`

then

`vagrant ssh`

then

`su - netrunner`

## Sources

https://www.hackthebox.com/hacker

https://github.com/CISOfy/Lynis?tab=readme-ov-file

https://docs.redhat.com/en-us/documentation/red_hat_enterprise_linux/8/pdf/security_hardening/Red_Hat_Enterprise_Linux-8-Security_hardening-en-US.pdf

https://overthewire.org/wargames/

https://hacker101.com

https://www.hackthis.co.uk/

https://www.root-me.org/?lang=en

https://www.reddit.com/r/hacking/comments/110fcop/how_to_stay_anonymous_online/
