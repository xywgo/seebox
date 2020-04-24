## Usage

### docker

```bash
docker run -d  \
    --name=flexget \
    -e PUID=1000 \
    -e PGID=1000 \
    -e TZ=Europe/London \
    -p 8600:8600 \
    -v </path/to/download/torrents>:/torrents \
    -v </path/to/appdata/config >:/config \
    -e WEBUI_PASSWD="YOURPASSWD" \
    xywgo/flexget
```
