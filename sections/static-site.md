##Exemplo simples - Site estático

**\$ docker run dockersamples/static-site**
(Quando não é uma imagem oficial precisamos identificar o username antes, nesse casom dockersamples)

**\$ docker run -d dockersamples/static-site**
(Roda o mesmo comando só que desatrelado ao meu terminal, não irá ficar travando o terminal)

**\$ docker run -d -P dockersamples/static-site**
(Atrela alguma porta aleatória gerada pelo docker do meu SO as portas usadas pelo container)

**$ docker port $ID_CONTAINER**
(Mostra quais portas estão mapeadas para as portas do container)

**\$ docker run -d -P --name meu-site dockersamples/static-site**
(Adiciona um name ao container)

**\$ docker run -d -p 12345:80 dockersamples/static-site**
(Mapea a porta 80 do container para a minha porta 12345)

**\$ docker run -d -e AUTHOR="Luiz Henrique" dockersamples/static-site**
(Seta uma variável de ambiente AUTHOR dentro do container)
