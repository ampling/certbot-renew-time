# certbot-renew-time

Silence those notification emails from expiry at letsencrypt dot com.

1) `$ ``git clone https://github.com/ampling/certbot-renew-time`
2) `$ ``cd certbot-renew-time`
2) `$ ``chmod +x ./certbot-renew-time`
3) `# ``sudo rsync ./certbot-renew-time /usr/local/bin/`
4) `# ``sudo rsync ./systemd/certbot-renew-time.service /etc/systemd/system/`
5) `# ``sudo rsync ./systemd/certbot-renew-time.timer /etc/systemd/system/`
6) `# ``sudo systemctl start certbot-renew-time.timer`
7) `# ``sudo systemctl enable certbot-renew-time.timer`

Tested daily against:  certbot, nginx, and systemd.
