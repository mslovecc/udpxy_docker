![Docker Image Size (tag)](https://img.shields.io/docker/image-size/dextercai/udpxy/latest)
![GitHub License](https://img.shields.io/github/license/dextercai/udpxy_docker)

# How To Use?

```bash
sudo docker stop udpxy
sudo docker rm udpxy
sudo docker run --name udpxy \
 --network host \
 --restart unless-stopped \
 -d mslovecc/udpxy:latest \
 -T -S -p 4022 -m enp1s0 -c 5 -B 256kb
```
Please change `enp1s0` to your local iface name.
