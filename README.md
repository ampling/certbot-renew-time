# certbot-renew-time

Lets encrypt is outstanding, but, receiving those expiry notifications emails and running the certbot renew manually gets old fast.  After reading the documentation more thoroughly, I found a setup which works for me and I've been asked to share.  This simple script should be safe to run daily. Web-server configurable. Additional email notifications are off by default.


```
$ git clone https://github.com/ampling/certbot-renew-time
$ cd certbot-renew-time
$ chmod +x ./certbot-renew-time
# rsync ./certbot-renew-time /usr/local/bin/
# rsync ./systemd/certbot-renew-time.service /etc/systemd/system/
# rsync ./systemd/certbot-renew-time.timer /etc/systemd/system/
# systemctl start certbot-renew-time.timer
# systemctl enable certbot-renew-time.timer
```

Tested daily against:  certbot, nginx, and systemd.
