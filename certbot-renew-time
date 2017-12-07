#!/usr/bin/env bash

web_server=nginx


sudo /usr/bin/certbot renew --quiet --agree-tos --pre-hook "service $web_server stop" --post-hook "service $web_server restart" >> /var/log/certbot-renew.log
# mail -s "CERTBOT Renewals" certbotrenew@example.com < /var/log/certbot-renew.log
exit 0
