# Tageler Docker Compose

## Quickstart

```bash
docker-compose pull
docker-compose up -d
```

## Configuration
```bash
sed -i \
  -e 's/VIRTUAL_HOST: api.tageler.ch/VIRTUAL_HOST: api.example.org/' \
  -e 's/VIRTUAL_HOST: www.tageler.ch/VIRTUAL_HOST: www.example.org/' \
  docker-compose.yml
```

## Development

```bash
sed -i \
  -e 's@tageler/tageler-api:latest@tageler/tageler-api:develop@' \
  -e 's@tageler/tageler-frontend:latest@tageler/tageler-frontend:develop@' \
  -e 's/VIRTUAL_HOST: api.tageler.ch/VIRTUAL_HOST: api.tageler.vcap.me/' \
  -e 's/VIRTUAL_HOST: www.tageler.ch/VIRTUAL_HOST: www.tageler.vcap.me/' \
  docker-compose.yml
```
