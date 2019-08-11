## Docker Host

```bash
docker -H ssh://root@xyz.com ps
docker -H ssh://root@xyz.com images

docker-compose -H ssh://root@xyz.com up
docker-compose -H ssh://root@xyz.com --help

docker -H ssh://root@xyz.com build .
docker -H ssh://root@xyz.com build -t wearetherock/dotnet-web-xyz .

docker -H ssh://root@xyz.com run \
    --name web \
    --rm  \
    -p 8888:80 \
    wearetherock/dotnet-web-xyz

open http://xyz.com:8888/api/values
```