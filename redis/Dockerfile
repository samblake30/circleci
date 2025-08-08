FROM komljen/ubuntu
LABEL maintainer="Alen Komljen <alen.komljen@live.com>"

RUN \
  apt-get update && \
  apt-get -y install \
          redis-server && \
  rm -rf /var/lib/apt/lists/*

RUN rm /usr/sbin/policy-rc.d
CMD ["/usr/bin/redis-server"]

EXPOSE 6379