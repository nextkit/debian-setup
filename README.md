# debian-setup
My debian setup

## Installation

### Docker
[Guide](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-debian-9)

### Github Actions service

Create file `/etc/systemd/system/github-actions.service` with content:  
  
**Service File**
```bash
[Unit]
Description=Starts and runs the github actions shell script

[Service]
Type=simple
User=<user-to-run-as> 
ExecStart=/<path-to-installation>/actions-runner/run.sh 
```

### Nginx Config

[Guide for Virtual Blocks](https://www.digitalocean.com/community/tutorials/how-to-set-up-nginx-server-blocks-virtual-hosts-on-ubuntu-16-04)
