FROM gcc2ge/geth_all:v0.2


WORKDIR "/root"


ENV nodekeyhex=""
CMD exec bootnode -nodekeyhex $nodekeyhex

EXPOSE 30301/udp
EXPOSE 30303/udp
