## TCP proxy for docker unix socket

Used to simulate docker integration with swarm
```bash
socat -d -d TCP4-LISTEN:2375,fork UNIX-CONNECT:/var/run/docker.sock
```
