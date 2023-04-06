# Introduction

# initalization

install and first env dependancy

```bash
mv .env.example .env
npm install | npx i --save-dev hasura-cli
```

add postgres connection string relative to docker container 
`postgresql://<user>:<pass>@postgres-hasura:5432/postgres`

migrate and populate hasura project

lunch hasura in console mode

```bash
cd hasura
npx hasura console --envfile .env.example
npx hasura deploy

# optionaly to stay updated
npx hasura migrate apply
npx hasura metadata apply
```
