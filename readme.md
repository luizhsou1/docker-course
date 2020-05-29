# **Curso de Docker - Alura**

> ## Instruções úteis

**\$ docker run hello-world**
(Baixa caso não tenha a imagem para criar um novo container)

**\$ docker ps**
(Tem todos os containers em execução nomomento)

**\$ docker ps -a**
(Tem Todos os containers criados, independetes de estarem em execução)

**\$ docker run -it ubuntu**
(Executa de forma iterativa, conecta o meu terminal ao terminal do ubuntu nesse caso)

**\$ docker start $NOME_CONTAINER ou $ID_CONTAINER**
(Starta um container parado)
obs.\$ID_CONTAINER pode ser só o começo que já identifica

**/\$ docker start -a -i ubuntu**
(Conecta(Atach) um container em execução e roda no modo interativo, para poder executar comandos)

**\$ docker stop $NOME_CONTAINER ou $ID_CONTAINER**
(Para um container ativo)
