FROM telegraf:1.30.0

MAINTAINER Yadir Rodriguez <yadirrh88@gmail.com>

RUN apt-get update && apt-get install -y unzip snmp-mibs-downloader && sed -i "s/^\(mibs *:\).*/#\1/" /etc/snmp/snmp.conf

COPY ./dlink/*.mib /usr/share/snmp/mibs/
