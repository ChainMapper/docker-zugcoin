# docker-zugzoin
Wallet and daemon for Zugzoin [ZCN] cryptocurrency on docker

# Quickstart
Type `docker run -it -e "USER=me" -e "PASSWORD=secret" -e "RPCALLOW=127.0.0.1" chainmapper/zugzoin` and see the wallet starting.

Alternatively type `docker run -it -v "<path_to_config>:/config/zugzoin.conf" chainmapper/zugzoin` to use your own config.

```
Docker ZCN wallet

By: ChainMapper
Website: https://chainmapper.com

Starting ZCN daemon...
```

# Proper start
Use a volume to store all data. The image stores it's data in `/data`. So mapping that volume will do the trick.

Additionally you can override the config and wallet file using volumes pointing to `/config/zugzoin.conf` and `/config/wallet.data`

# License
MIT, see LICENSE file