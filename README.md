# docker-mac-network

In case of Docker on MAC, the host doesn't have direct access to the docker network. 
Due to this, the services running in docker container cannot be accessed directly via
their IP addresses. One of the solution is to create a VPN between the host and the
docker network.

 ### Create a VPN
```bash
curl -sL https://raw.githubusercontent.com/mesosphere/docker-mac-network/master/mac-network.sh | bash -s create
```

 ### Destroy the VPN
```bash
curl -sL https://raw.githubusercontent.com/mesosphere/docker-mac-network/master/mac-network.sh | bash -s destroy
```
