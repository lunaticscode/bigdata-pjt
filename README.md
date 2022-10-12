## Version

- OS: Centos6 (CM과 Agent 모두 동일.)
- Java: JDK 1.8
- ClouderaManager: 3.7x

#

## Docker Container setting

```bash
$ docker-compose up -d
```

#

## Hadoop-CM setting

```bash
$ vi /etc/hosts
```

```bash
...

# hadoop cm, agent host 정보 추가 (Docker-compose.yml 파일 참고)
{docker-01-ip}  {docker-01-hostname}
{docker-02-ip}  {docker-02-hostname}
{docker-03-ip}  {docker-03-hostname}

...
```

```bash
$ wget https://archive.cloudera.com/cloudera-manager_372/installer/latest/cloudera-manager-installer.bin
$ chmod u+x ./cloudera-manager-installer.bin
$ ./cloudera-manager-installer.bin
```

- localhost:7180 으로 접속
