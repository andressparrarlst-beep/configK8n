Usar el siguiente comando para poner la variables de entorno llamado `secret` en kubernetes

```
kubectl create secret generic uptc-secrets \
  --from-literal=DB_PASSWORD=1234 \
  --from-literal=DB_URL=jdbc:postgresql://postgres-service:6432/uptc_db \
  --from-literal=DB_USER=postgres
```