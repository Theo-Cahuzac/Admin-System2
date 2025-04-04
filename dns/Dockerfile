FROM internetsystemsconsortium/bind9:9.18

COPY named.conf /etc/bind/named.conf

COPY l2-9.zone /etc/bind/zone/l2-9.zone

RUN apk update && apk add nano

RUN chown -R bind:bind /etc/bind /var/cache/bind /var/log && \
    chmod -R 770 /etc/bind /var/cache/bind /var/log /etc/bind/zone


