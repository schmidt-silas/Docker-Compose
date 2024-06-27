create acme.json
```
touch volume/acme.json
chmod 600 volume/acme.json
```
ACME E-Mail manuel anpassen
```
nano volume/traefik.yml
```

Befeht password hash für .env & rest anpassen
```
sudo apt install apache2-utils
```
```
echo $(htpasswd -nb "user" "pw") | sed -e s/\\$/\\$\\$/g
```
```
nano .env
```
docker starten

```
docker compose up -d
docker compose logs
```

DNS Record auf traefik.[domain]