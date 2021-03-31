#!/bin/sh
set -e

htpasswd -bBc /etc/nginx/.htpasswd $BASIC_AUTH_USERNAME $BASIC_AUTH_PASSWORD

exec nginx -g "daemon off;"
