# Consul 0.5.0 Docker image
Based on the busybox:ubuntu-14.04 image.
The .tar.gz archive in this repo is directly converted from the zip file from the [Consul download page](https://www.consul.io/downloads.html) using

```
unzip -p 0.5.0_linux_amd64.zip
tar -zcvf consul.tar.gz consul
```

## How to use

```
docker run -ti cargonauts/consul:0.5.0 /consul <OPTIONS>
```

Or build your own image using `cargonauts/consul:0.5.0` as your base image.
