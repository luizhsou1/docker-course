## Comunicação entre Containers

Por padrão todos os containers criados no docker, estão funcionando em uma mesma rede.
Exemplo: - Redis 172.168.0.1 - Mongo 172.168.0.2 - Node 172.168.0.3
Mas isso não é o ideal, pois por padrão o docker não atribui um hostname, logo é difícil trabalhar diretamente por IPs. Uma solução para isso é criar minha própria rede.

**\$ docker network create --driver bridge minha-rede**
(Cria uma rede)

**\$ docker network ls**
(Lista todas as redes)

**\$ docker run -it --name meu-container-ubuntu --network minha-rede ubuntu**
(cria um container do ubuntu e atrela ele a minha-rede, e agora posso comunicar os containers pelo hostname)
