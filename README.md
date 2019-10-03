### zulu-openjdk
---
https://github.com/zulu-openjdk/zulu-openjdk/blob/master/8-latest/README.md

https://github.com/zulu-openjdk

```dockerfile
FROM ubuntu:16.04

RUN apt-get -qq update && \
  apt-get -qqy install locales && \
  locale-gen en_US.UTF-8 && \
  rm -rf /var/lib/apt/lists/*
  
ENV LANG en_US.UTF-8
ENV LANGUAGE en_US:en
ENV LC_ALL en_US.UTF-8

RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys xxx && \
    echo "deb http://repose.zulsystem.com/ubuntu stable main">> /etc/apt/sources/list.d/zulu.list && \
    apt-get -qq update &&\
    apt-get -qqy install zulu-9 && \
    rm-rf /var/lib/apt/lists/*
```

```
```

```
```


