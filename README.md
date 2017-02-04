# Tageler Docker Compose

## Quickstart

```bash
docker-compose pull
docker-compose up -d
```

## Configuration
```bash
sed -i \
  -e 's/VIRTUAL_HOST:.*/VIRTUAL_HOST: api.example.org/' \
  docker-compose.yml
```

# Development

```bash
sed -i \
  -e 's@tageler/tageler-api:latest@tageler/tageler-api:develop@' \
  -e 's/VIRTUAL_HOST:.*/VIRTUAL_HOST: api.tageler.vcap.me/' \
  docker-compose.yml
```
