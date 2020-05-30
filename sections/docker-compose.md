## Trabalhando com Docker Compose

Ele irá orequestrar o fluxo de subida e execução da aplicação, com base no arquivo docker-compose.yml.

**\$ docker-compose build**
(Builda o arquivo docker-compose.yml, criando todas as imagens descritas)

**\$ docker-compose up**
(Executa as imagens criadas no build na ordem correta)

**\$ docker-compose up -d**
(Executa as imagens criadas no build na ordem correta, só que em background)

**\$ docker-compose ps**
(Lista todos os containers daquela build em execução)

**\$ docker-compose down**
(Para todos os containers e os remove, logo não ficaram parados)
