# certbot-renew-time

Silence those notification emails from expiry at letsencrypt dot com.

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
