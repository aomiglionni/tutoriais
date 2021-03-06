# Comandos úteis sobre Docker

## Procurar a imagem
### docker search ubuntu

## Baixar uma imagem
### docker pull ubuntu

## Listar imagens
### docker images

## Remover imagem
### docker rmi ID_ou_nome_da_imagem

## Criar um container
### docker run nome_da_imagem

## Criar um container e entrar no terminal
### docker run -it ubuntu /bin/bash

## Criar um container com um nome
### docker run --name meu_ubuntu ubuntu

## Verificar o estado ou encontrar o ID do container (somente em atividade)
### docker ps

## Verificar todos os containers
### docker ps -a
### docker ps -qa

## Remover um container
### docker rm id_ou_apelido

## Informações úteis de um container
### docker stats id_ou_apelido

## Informações sobre o container
### docker inspect id_ou_apelido

## Commitar alterações em uma imagem
### docker commit ID/apelido nome_da_nova_imagem

## Mapear uma porta para o container
### docker run -it -p 8080:80 ubuntu

## Montar containers auto destrutivos (ao sair da sessão é destruído)
### docker run -it --rm -p 8080:80 nginx /bin/bash

## Executar container em segundo plano
### docker run -d -p 8080:80 nginx /usr/sbin/nginx -g

## Parar um container
### docker stop id_ou_apelido

## Iniciar um container
### docker start id_ou_apelido

## Remover todos os containers
### docker rm $(docker ps -qa)

## Remover todas as imagens
### docker rmi $(docker images -q)

## Executar comandos sem precisar estar dentro do container
### docker exec -it id_ou_apelido comando
### docker exec -it ubuntinho ifconfig eth0
### docker exec -it nginx_teste ls -lh

## Acesso ao bash
### docker exec -it nginx_teste bash






