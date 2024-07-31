This is for using N1MM distrubted.

Server Config: 
Note: Server needs to have an exposed  public ipv4 address.
1. Install Docker on server. 
```
curl -sSL https://get.docker.com | sh
sudo usermod -aG docker $(whoami)
```
2. edit container configs. in docker-compose.yml

3. Run docker container
```
docker compose up -d
```

4. Make sure that the host file is located in the ./hosts/ directory. 

5. Head to web ui at `http://{{ip.address}}:51834`

Client Config: Please read Client Config File.


References:
[wg-easy](https://github.com/wg-easy/wg-ea0sy)
[N1MM Logger ](https://n1mmwp.hamdocs.com/)
