This is for using N1MM distrubted.

Server Config: 
Note: Server needs to have an exposed public ipv4 address and the 2 ports (51834, 51820)
1. Install Docker on server. 
```
curl -sSL https://get.docker.com | sh
sudo usermod -aG docker $(whoami)
```
2. Determine your public ip address.
```
curl ifconfig.me
```
2. add config file to server
```
git clone https://github.com/kd9lsv/n1mm_multi_distrubted.git && cd n1mm_multi_distrubted
```
3. edit container configs. in [docker-compose.yml](./docker-compose.yml)

4. Run docker container
```
docker compose up -d
```

5. Make sure that the host file is located in the ./hosts/ directory. 

6. Head to web ui at `http://{{ip.address}}:51834`

Client Config: Please read Client [Config File](./Client_VPN_Config.pdf).


References:
[wg-easy](https://github.com/wg-easy/wg-ea0sy)
[N1MM Logger ](https://n1mmwp.hamdocs.com/)
