# Postgres Deploy

Deploys a simple 3 node postgres server.  Utilizes external secrets operator

## Prereqs

Doppler service token needs to be seeded for external secrets operator by being place in a secret


```
kubectl create secret generic doppler-token-postgres-deploy -n external-secrets --from-literal dopplerToken="dp.st...."
```


## Adminer

Adminer is a gui for interacting with postgres