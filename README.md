# Instruction of building a SOLARSITE mini-pc platform for energy monitoring and control, hardware access

Since Kubernetes is designed to be mostly hardware agnostic, it is not very strong in exploiting the server hardware
resources. For this reason we will add a Docker container runtime environment to fill-in these functional gaps.


## Component choices
```
**Software**:
```markdown
1. Docker https://www.docker.com
2. NodeRed https://nodered.org/
3. FTP server https://hub.docker.com/r/garethflowers/ftp-server
```

## Installation

### Docker

Installing Docker is easy

`sudo apt install docker.io -y`

Check that Docker is running properly

`sudo service docker status`

*reference articles*

>[Installing docker](https://mariadb.com/resources/blog/building-a-portable-database-server/)

### Docker-compose

Next we will create a 