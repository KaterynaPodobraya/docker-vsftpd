# docker-vsftpd [![Docker Build Status](https://img.shields.io/docker/build/stellarity/vsftpd.svg)](https://hub.docker.com/r/stellarity/vsftpd)

## Config
`MODE`:
- FTP
- FTPS
- FTPES

`PASV_ADDRESS`

### Users
| username | password |
|--|--|
| one | one |
| two | <none> |
| anonymous | <none> |

## Run

```bash
MODE=FTP PASV_ADDRESS=192.168.2.156 docker-compose up
```

## Debug run

```bash
docker-compose run --service-ports --rm -e PASV_ADDRESS=192.168.2.156 -e MODE=FTP vsftpd
```
