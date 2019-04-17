FROM gcc2ge/geth_all:v0.2


WORKDIR "/root"

ARG password
ARG privatekey
RUN echo $password > ~/.accountpassword
RUN echo $privatekey > ~/.privatekey


RUN geth account import --password ~/.accountpassword  ~/.privatekey

ENV address=""
ENV bootnodeId=""
ENV bootnodeIp=""

CMD exec geth --bootnodes "enode://$bootnodeId@$bootnodeIp:30301" --networkid "6660001" --verbosity=4 --rpc --rpcaddr "0.0.0.0" --rpcapi "eth,web3,net,admin,debug,db" --rpccorsdomain "*" --mine --etherbase $address --unlock $address --password ~/.accountpassword
