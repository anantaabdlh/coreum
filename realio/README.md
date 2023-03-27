<h3><p style="font-size:14px" align="right">Founder :
<a href="https://discord.gg/nodexcapital" target="_blank">NodeX Capital Discord Community</a></p></h3>
<h3><p style="font-size:14px" align="right">Visit Our Website :
<a href="https://discord.gg/nodexcapital" target="_blank">NodeX Capital Official</a></p></h3>
<h3><p style="font-size:14px" align="right">Hetzner :
<a href="https://hetzner.cloud/?ref=bMTVi7dcwSgA" target="_blank">Deploy Hetzner VPS Get 20€ Bonus!</a></h3>
<hr>

<p align="center">
  <img height="100" height="auto" src="https://raw.githubusercontent.com/Nodeist/Kurulumlar/main/logos/realio.png">
</p>

# Realio Network Testnet | Chain ID : realionetwork_3300-1 | Custom Port : 231

### Community Documentation:
>- https://nodeist.net/t/Realio/

### Explorer:
>-  https://explorer.nodexcapital.com/realio

### Automatic Installer
You can setup your Realio Network fullnode in few minutes by using automated script below.
```
wget -O realio.sh https://raw.githubusercontent.com/nodexcapital/testnet/main/realio/realio.sh && chmod +x realio.sh && ./realio.sh
```
### Public Endpoint

>- API : https://rest.realio-t.nodexcapital.com
>- RPC : https://rpc.realio-t.nodexcapital.com
>- gRPC : https://grpc.realio-t.nodexcapital.com

### Snapshot (Update every 5 hours)
```
COMING SOON
```

### State Sync
```
COMING SOON
```

### Live Peers
```
PEERS="$(curl -sS https://rpc.realio-t.nodexcapital.com/net_info | jq -r '.result.peers[] | "\(.node_info.id)@\(.remote_ip):\(.node_info.listen_addr)"' | awk -F ':' '{print $1":"$(NF)}' | sed -z 's|\n|,|g;s|.$||')"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.realio-network/config/config.toml
```
### Addrbook (Update every hour)
```
COMING SOON
```
### Genesis
```
COMING SOON
```