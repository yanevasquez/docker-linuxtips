
#### Dockerfile

**1. Descrição geral do [dockerfile 01](https://github.com/yanevasquez/docker-linuxtips/dockerfiles/01/Dockerfile):**

```dockerfile
FROM ← imagem ao qual o container é baseado.

RUN ← os comandos são executado quando estiver 'buildando' a imagem, é criado uma camada a cada RUN.
Então, o uso do && permite não criar camadas novas.

ENV ← é possível adicionar variáveis de ambiente necessárias para executar o apache.

LABEL ← adicionar metadados. 

VOLUME ← volume setando um nome sem hash, não é possível ser tipo bind.

EXPOSE ← a porta que está em execução.
```

##### 2. Fazer build da imagem com tag:

```sh
docker image build -t meu_apache:1.0.0 .
```
##### 3. Outros comandos: 

```sh
du -sh * => verifica o tamanho dos arquivos. 
```
...

