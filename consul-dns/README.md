# Consul as DNS server
Based on our [cargonauts/consul image](https://registry.hub.docker.com/u/cargonauts/consul/), configured for:
- DNS server at port 53
- Recursor to Google's 8.8.8.8 DNS server


## How to use
```
# Run the Consul DNS container
docker run -d -p <DOCKER0_IP>:53:53/udp cargonauts/consul-dns
# for example
docker run -d -p 172.17.42.1:53:53/udp cargonauts/consul-dns
```
