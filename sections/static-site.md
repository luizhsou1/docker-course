##Exemplo simples - Site estático

**\$ docker run dockersamples/static-site**
(Quando não é uma imagem oficial precisamos identificar o username antes, nesse casom dockersamples)

**\$ docker run -d dockersamples/static-site**
(Roda o mesmo comando só que desatrelado ao meu terminal, não irá ficar travando o terminal)

**\$ docker run -d -P dockersamples/static-site**
(Atrela alguma porta do meu SO as portas usadas pelo container)
