# Consul as DNS server w/ web ui

Based on our [cargonauts/consul-dns image](https://registry.hub.docker.com/u/cargonauts/consul-dns/), configured for:
- DNS server at port 53
- Web UI at port 8500

The .tar.gz archive in this repo is directly converted from the zip file from the [Consul download page](https://www.consul.io/downloads.html) using

```
unzip 0.5.0_web_ui.zip
tar -zcvf 0.5.0_web_ui.tar.gz dist
```


## How to use
```
# Run the Consul DNS container
docker run -d -p 53:53/udp -p 8500:8500 cargonauts/consul-web
```
