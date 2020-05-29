## Usando os volumes

Serve basicamente para conseguir persistir os dados, então independente de remover aquele container os dados persistirão.
Pois as pastas criadas como volumes ficam não no container e sim num lugar reservado no docker host (cara que gerencia os containers para mim), e apenas mapeia para dentro do container.

**\$ docker run -v "/var/www" ubuntu**
(Cria um container do ubuntu com um volume em /var/www)

**\$ docker inspect $NOME_CONTAINER ou \$ID_CONTAINER**
(Mostra tudo relacionado ao container, mas para essa seção, olhe o atributo Mounts, lá irá aparecer o source (lugar na máquina host onde efetivamente persistirá a pasta) e o Destination (Pasta mapeada no container))

**\$ docker run -v "\$ANY_PATH:/var/www"**
(Altero o caminho padrão de persistir os volumes para um path qualquer que passar)

**\$ docker run -d -p 8080:3000 -v "/home/luiz/git/hub/my/docker-course/volume-exemplo:/var/www" -w /var/www" node npm start**
(Mapea um diretório local para um diretório dentro do container, útil para executar coisas que não tenho dentro do container, exemplo, baixei um fonte de exemplo em PHP, mas não quero instalar na minha máquina, baixo a imagem do PHP e coloco o container para enxergar a pasta local do projeto, para conseguir executar)

**flags Aprendidas**
-w: Fala qual diretório é para ser executado o comando
