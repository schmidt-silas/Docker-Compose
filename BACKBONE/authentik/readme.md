add variable to ENV
```
echo "PG_PASS=$(openssl rand -base64 36 | tr -d '\n')" >> .env
echo "AUTHENTIK_SECRET_KEY=$(openssl rand -base64 60 | tr -d '\n')" >> .env
```
optional Debugging
```
echo "AUTHENTIK_ERROR_REPORTING__ENABLED=true" >> .env
```

INITIAL SETUP !!

https://<your Domain>/if/flow/initial-setup/

DefaultUser: akadmin