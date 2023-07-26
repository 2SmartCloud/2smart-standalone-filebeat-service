# 2smart-filebeat

To build multi-platform image use `Dockerfile.mutilatofirm` and buildx:

```bash
docker buildx build \
    --file ./Dockerfile.multiplatform \
    --platform=linux/amd64,linux/arm/v7 \
    -t gitlab.iot.webbylab.com:5050/2smart/standalone/services/filebeat
```