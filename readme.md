#### Comandos e termos gerais:

#### 1.Container: 
- É uma parte isolada do sistema operacional
  - isolamento físico 
  - isolamento lógico


##### Visualizar todos os containers que foram criados, ativos ou inativos.  

```
docker container ls -a
```

 - Na construção de uma imagem é criado uma camada ao executar algum processo. Todas as camadas são read-only, exceto a última que será sempre read-write.

 ##### Rodar com o terminal interativo **-ti** : 

```
 docker container run -ti ubuntu
``` 
##### Sair do container sem matar o processo : 

```
ctrl pq
``` 
##### Listagens: 
```
 docker image ls
 docker ps
 docker container ls
 docker container ls -a
```

##### Voltar para um container em execução:
```
 docker container attach [CONTAINER ID]
```
##### Rodar no modo daemon(rodar em background), por isso utiliza a flag -d: 

```
 docker container -d nginx
``` 

##### Conectar processos em background:
```
docker container exec -ti [CONTAINER ID] [COMANDO]
``` 

##### Manipular status do container:
```
docker container start [CONTAINER ID]
docker container stop [CONTAINER ID]
docker container restart [CONTAINER ID]
docker container pause [CONTAINER ID]
docker container unpause [CONTAINER ID]
``` 
##### Identificar consumo de CPU e memória
```
 docker container stats [CONTAINER ID]
 ``` 



