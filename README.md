# certbot-renew-time

There are many ways to setup certbot to enable automatic renewal of your Let's Encrypt SSL/ TLS certifications. This sample configuration should work well with any modern Linux stack utilizing the power of systemd timers.


**Features:**
* Safe to run daily. 
* Web-server configurable. (restarts only when needed)
* Email notifications. (optional)


## Installation
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
