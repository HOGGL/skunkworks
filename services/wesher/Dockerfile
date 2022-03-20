FROM balenalib/armv7hf-debian

WORKDIR /
RUN install_packages wget miniupnpc dnsutils inotify-tools
RUN wget -O wesher https://github.com/costela/wesher/releases/latest/download/wesher-arm
COPY run.sh run.sh
COPY hosts_updated.sh .
COPY watch_hosts.sh .
CMD [ "/run.sh" ]