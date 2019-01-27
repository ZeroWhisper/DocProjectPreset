
# Download docker on https://hub.docker.com/

* List command

## To do LOGIN on Docker
```sh
docker login
```

# Processo ou ciclo de vida do Docker (Precisa melhorar)

 - Baixar a image
 - Copiar os arquivos necessários para a imagem
 - Ter o arquivo .yaml com a configuração da imagem
 - Subir a imagem
 - [Trabalhar com a imagem] Derrubar a imagem
 
# Docker usado para banco de dados postgres no Curso da Rocketseat
docker run --name database -p 5432:5432 -d -t kartoza/postgis
Outra imagem: postgres:alpine

# Command

## Help
```sh
docker container --
```
```sh
docker imagem --help
```

## Image Basic
 - Baixa a imagem solicitada, este comando pode ser executado implicitamente, quando o docker
precisa de uma imagem para outra operação e não consegue localiza-la no cache local.
```sh
docker image pull <tag>
```
 - Lista todas as imagens já baixadas
```sh
docker image ls
```
 - Remove uma imagem do cache local
```sh
docker image rm <tag>
```
 - Extrai diversas informações utilizando um formato JSON da imagem indicada
```sh
docker image inspect <tag>
```
 - Cria/Copia uma nova tag baseada em uma tag anterior ou hash.
```sh
docker image tag <source> <tag>
```
 - Permite a criação de uma nova imagem
```sh
docker image build -t <tag>
```
 - Permite o envio de uma imagem ou tag local para um registry.
```sh
docker image push <tag>
```

Extra:
 - A linha de comando para procurar imagens no Docker Hub
```sh
docker search <tag> 
```

# Docker Composer
Descrição: Comando para executar uma sério de containers a partir de um arquivo .yaml

 - Exemplo de arquivo: docker-compose.yml — Apenas o serviço de front-end
```yaml
frontend:
    image: nginx:1.13
    volumes:
    # Site
    - ./web:/usr/share/nginx/html/
    ports:
    - 80:80
```

```sh
docker-compose up -d
docker-compose logs -f -t
```

## RUN














