# geth_ipos

替换geth中POW算法替换成POS共识算法，这里提供的是项目的镜像。

### 运行项目

1. clone项目

```
git clone https://github.com/gcc2ge/blockchain_tps.git
```

2. docker-compose运行镜像

```
docker-compose up -d
```

3. 查看运行中的容器 

```
docker ps


CONTAINER ID        IMAGE                        COMMAND                  CREATED             STATUS              PORTS                                                                                             NAMES
611a90e3111a        geth-ipos_geth-dev-node      "/bin/sh -c 'exec ge…"   About an hour ago   Up About an hour    0.0.0.0:8545->8545/tcp, 0.0.0.0:30303->30303/tcp, 8546/tcp, 0.0.0.0:30303->30303/udp, 30304/udp   geth-node
265bfd6b6f05        geth-ipos_geth-dev-miner-3   "/bin/sh -c 'exec ge…"   About an hour ago   Up About an hour    8545-8546/tcp, 30303/tcp, 30303-30304/udp                                                         geth-miner-3
ef33ec752de0        geth-ipos_geth-dev-miner-1   "/bin/sh -c 'exec ge…"   About an hour ago   Up About an hour    8545-8546/tcp, 30303/tcp, 30303-30304/udp                                                         geth-miner-1
30bf577473f3        geth-ipos_geth-dev-miner-2   "/bin/sh -c 'exec ge…"   About an hour ago   Up About an hour    8545-8546/tcp, 30303/tcp, 30303-30304/udp                                                         geth-miner-2
4244a6402c65        geth-ipos_geth-bootnode      "/bin/sh -c 'exec bo…"   About an hour ago   Up About an hour    8545-8546/tcp, 30303/tcp, 0.0.0.0:30301->30301/udp, 30303-30304/udp                               geth-ipos_geth-bootnode_1
```

如果想测试geth_ipos的tps，可以查看[blockchain_tps](https://github.com/gcc2ge/blockchain_tps)项目，这里提供测试TPS的相关工具
