# sgnome-cm
Configuration Management for Steam Gnome

## ENV Example
```
STEAM_API_KEY="YOUR STEAM KEY HERE"
REDIS_HOST="redis"
STEAM_API_URL="http://steamapi:3000"
```

## Run SGNOME
`docker-compose --env-file .env -f config/dev/infrastructure.yml -f config/dev/sgnome.yml up -d`

- Navigate to `localhost:5540` and create a new database if needed
- Select the pub/sub button on the left sidebar
- Hit the subscribe button
- Send a message on `channel: SGNOME/vanityurl`, `payload: { "vaniturl": "ac89" }`

