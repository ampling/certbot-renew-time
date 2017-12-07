# certbot-renew-time

Silence those notification emails from expiry@letsencrypt.com.

1) git clone https://github.com/ampling/certbot-renew-time
2) cd certbot-renew-time
2) chmod +x ./certbot-renew-time
3) rsync ./certbot-renew-time /usr/local/bin/
4) rsync ./systemd/certbot-renew-time.service /etc/systemd/system/
5) rsync ./systemd/certbot-renew-time.timer /etc/systemd/system/
6) systemctl start certbot-renew-time.timer
7) systemctl enable certbot-renew-time.timer

Tested daily against:  certbot, nginx, and systemd.
