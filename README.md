# e2e

![color](https://img.shields.io/static/v1?label=e2e&message=I9XP.Tecnologia&color=yellow)

Sistema para automatização de testes

## Requisitos
* NVM - Pode ser que precise variar entre as versões **14.15.4** e **12** do node
* NodeJS - **14.15.4**
* NPM
* Docker **engine** e **docker compose**

## Inicialização

Crie uma pasta raiz (e2e/ por exemplo) e clone todas as aplicações dentro da mesma

```bash
mkdir e2e && cd e2e
```

```bash
git clone ...
```

## Start Docker
Entre na pasta docker-builder e execute o seguinte

```bash
docker-compose up -d
```
Verifique se todos os containers estão rodando
```bash
docker ps
```

## Hosts
Adicione no arquivo hosts. Lembre-se de atribuir as portas definida dentro dos arquivos .env
```
localhost api.e2e.local:3000 (ou a porta definida no .env)
localhost dashboard.e2e.local:8080 (ou a porta definida no .env)
localhost mongoclient.e2e.local:3300 (ou a porta definida no .env)
```
Acesse para ver o resultado:
* [api.e2e.local:3000](api.e2e.local:3000) (ou a porta definida no .env)
* [dashboard.e2e.local:8080](dashboard.e2e.local:8080) (ou a porta definida no .env)
* [mongoclient.e2e.local:3300](mongoclient.e2e.local:3300) (ou a porta definida no .env)



