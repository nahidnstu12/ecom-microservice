# practical-microservice-workshop

prisma init: `npx prisma init --datasource-provider postgresql `

Email Service : http://localhost:8025/
PgAdmin: http://localhost:5050/browser/
Redis Stack: http://localhost:8002/redis-stack/browser


Service
---------
User Service: 4000
Product: 4001
Inventory: 4002
Auth: 4003
Cart: 4004
Email: 4005
Order: 4007

Api Gateway: 8081







## Run Kong and necessary services

```bash
cd kong-docker-compose && docker compose -f .\kong-docker-compose.yml up
```

## Run Keycloak

```bash

cd docker keycloak-docker-compose && docker compose -f ./keycloak-docker-compose.yml up
```

## Run microservices dependency

```bash
docker compose up
```
