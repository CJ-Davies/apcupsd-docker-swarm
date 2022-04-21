FROM alpine:latest

RUN apk update && apk add --no-cache bash apcupsd

COPY ./apcupsd.conf /etc/apcupsd/apcupsd.conf
COPY ./entrypoint.sh /usr/local/bin/entrypoint.sh

CMD ["/usr/local/bin/entrypoint.sh"]
