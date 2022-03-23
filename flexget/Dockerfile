FROM python:alpine
LABEL maintainer="xywgo"
LABEL version="3.3.3"

RUN \
    echo "**** install flexget ****" && \
    apk add --no-cache --virtual  .build-deps gcc g++ musl-dev linux-headers && \
    pip3 install -U pip && pip3 install flexget && \
    apk del .build-deps gcc musl-dev




# Copy local files
COPY root/  /

# ports and volumes
EXPOSE 8600 8600/tcp
VOLUME /config /torrents
