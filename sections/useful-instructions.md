## Instruções úteis

**\$ docker run hello-world**
(Baixa caso não tenha a imagem para criar um novo container)

**\$ docker ps**
(Tem todos os containers em execução nomomento)

**\$ docker ps -a**
(Tem Todos os containers criados, independetes de estarem em execução)

**\$ docker ps -q**
(Lista apenas os ids dos containers em execução)

**\$ docker run -it ubuntu**
(Executa de forma iterativa, conecta o meu terminal ao terminal do ubuntu nesse caso)

**\$ docker start $NOME_CONTAINER ou $ID_CONTAINER**
(Starta um container parado)

**/\$ docker start -a -i ubuntu**
(Conecta(Attach) um container em execução e roda no modo interativo, para poder executar comandos)

**\$ docker stop $NOME_CONTAINER ou $ID_CONTAINER**
(Para um container ativo)

**\$ docker stop -t 0 $NOME_CONTAINER ou $ID_CONTAINER**
(Para um container ativo, e não espera nem um segundo para isso, por padrão é 10)

**\$ docker stop \$(docker ps -q)**
(Para todos os containers em execução)

**\$ docker rm $NOME_CONTAINER ou $ID_CONTAINER**
(Remove um container especifíco)

**\$ docker container prune**
(Remove todos os containers inativos)

**\$ docker images**
(Mostra todas as imagens)

**\$ docker rmi $NOME_CONTAINER ou $ID_CONTAINER**
(Remove uma imagem específica)

**obs.\$ID_CONTAINER pode ser só o começo que já identifica**
