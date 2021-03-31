FROM nginx:1.19.9-alpine

# for htpasswd command
RUN apk add --no-cache --update \
      apache2-utils
RUN rm -f /etc/nginx/conf.d/*

COPY certs/domain.crt /etc/nginx/certs/
COPY certs/domain.key /etc/nginx/certs/
COPY run.sh /
COPY nginx.conf /etc/nginx/

ENTRYPOINT ["/run.sh"]
