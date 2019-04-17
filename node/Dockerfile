FROM gcc2ge/geth_all:v0.2


WORKDIR "/root"


ENV bootnodeId=""
ENV bootnodeIp=""

CMD exec geth --bootnodes "enode://$bootnodeId@$bootnodeIp:30301" --networkid "6660001" --verbosity=4 --rpc --rpcaddr "0.0.0.0" --rpcapi "eth,web3,net,admin,debug,db" --rpccorsdomain "*"  --syncmode="full"

EXPOSE 8545
EXPOSE 30303
