## Usando os volumes

Serve basicamente para conseguir persistir os dados, então independente de remover aquele container os dados persistirão.
Pois as pastas criadas como volumes ficam não no container e sim num lugar reservado no docker host (cara que gerencia os containers para mim), e apenas mapeia para dentro do container.

**\$ docker run -v "/var/www" ubuntu**
(Cria um container do ubuntu com um volume em /var/www)

**\$ docker inspect $NOME_CONTAINER ou \$ID_CONTAINER**
(Mostra tudo relacionado ao container, mas para essa seção, olhe o atributo Mounts, lá irá aparecer o source (lugar na máquina host onde efetivamente persistirá a pasta) e o Destination (Pasta mapeada no container))

**\$ docker run -v "\$ANY_PATH:/var/www"**
(Altero o caminho padrão de persistir os volumes para um path qualquer que passar)
