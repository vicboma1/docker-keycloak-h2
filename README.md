# docker-keycloak-h2

```
  keycloak:
    container_name: local_keycloak
    environment:
      KEYCLOAK_ADMIN: admin
      KEYCLOAK_ADMIN_PASSWORD: admin
      DB_VENDOR: h2
      DB_ADDR: h2
      DB_DATABASE: keycloak
      DB_USER: keycloak
      DB_PASSWORD: keycloak
    image: jboss/keycloak:13.0.0
    ports:
      - "28080:8080"
    restart: unless-stopped
```
