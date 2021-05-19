# 🟢 DJANGO

## Projeto linha-montagem-app-api-proxy

  > Proxy para aplicação linha-montagem-api-devops, com pipeline no Gitlab

- Modelo de versionamento **branch** e **tag release** (*-release)

## Usage

### Environment Variables

- `LISTEN_PORT` - Port to listen on (default: `8000`)
- `APP_HOST` - Hostname of the app to forward requests to (default: `app`)
- `APP_PORT` - Port of the app to forward requests to (default: `9000`)

### Running local machine

´´´shell
cd /linha-montagem-app-api-proxy
docker build -t proxy-lm .
cd ../linha-montagem-api-devops
docker-compose -f docker-compose-proxy.yml up
´´´

- Test: <http://localhost:8000/admin/>
