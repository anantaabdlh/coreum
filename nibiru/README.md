<h3><p style="font-size:14px" align="right">Founder :
<a href="https://discord.gg/bDUAwZhqBb" target="_blank">NodeX Capital Discord Community</a></p></h3>
<h3><p style="font-size:14px" align="right">Visit Our Website :
<a href="https://nodexcapital.com" target="_blank">NodeX Capital Official</a></p></h3>
<h3><p style="font-size:14px" align="right">Hetzner :
<a href="https://hetzner.cloud/?ref=bMTVi7dcwSgA" target="_blank">Deploy Hetzner VPS Get 20€ Bonus!</a></h3>
<hr>

<p align="center">
  <img height="100" height="auto" src="https://user-images.githubusercontent.com/44331529/199216266-6b0da979-44a2-43e4-b9ef-de3a7c361b17.png">
</p>

# Nibiru Testnet | Chain ID : nibiru-testnet-2 | Custom Port : 203

### Community Documentation:
>- https://nibiru.fi/
>- https://github.com/NibiruChain

### Explorer:
>-  https://explorer.nodexcapital.com/nibiru

### Automatic Installer
You can setup your Nibiru fullnode in few minutes by using automated script below.
```
wget -O nibiru.sh https://raw.githubusercontent.com/nodexcapital/testnet/main/nibiru/nibiru.sh && chmod +x nibiru.sh && ./nibiru.sh
```
### Public Endpoint

>- API : https://api.nibiru.nodexcapital.com
>- RPC : https://rpc.nibiru.nodexcapital.com
>- gRPC : https://grpc.nibiru.nodexcapital.com
>- gRPC Web : https://grpc-web.nibiru.nodexcapital.com

### Snapshot
```
COMING SOON
```

### State Sync
```
COMING SOON
```

### Live Peers
```
PEERS="$(curl -sS https://rpc.nibiru-t.nodexcapital.com/net_info | jq -r '.result.peers[] | "\(.node_info.id)@\(.remote_ip):\(.node_info.listen_addr)"' | awk -F ':' '{print $1":"$(NF)}' | sed -z 's|\n|,|g;s|.$||')"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$PEERS\"|" $HOME/.nibid/config/config.toml
```
### Addrbook
```
COMING SOON
```
### Genesis
```
COMING SOON
```