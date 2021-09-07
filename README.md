Sistema Gerenciamento Sala Reuniões
===========================
#### Descrição da atividade
Live Coding Desenvolvimento de um Sistema de Gerenciamento de Sala de Reuniões

Códigos desenvolvidos em treinamento da plataforma de ensino da Digital Innovation One, ministrado por [Kamila Santos](https://www.linkedin.com/in/kamila-santos-oliveira/ "Kamila Santos") desenvolvedora backend em [Ame Digital](https://www.linkedin.com/company/ame-digital/ "Ame Digital").
Esse repositório é dividido em duas pastas compactadas, uma contém o backend [back-room] da aplicação e a outra o frontend [client-room].

Endpoints API Sala

| Endpoints | Method | Describe |
| :---: | :---: | :---: |
| /api/v1/rooms | POST | Criar |
| /api/v1/rooms | GET | Listar  |
| /api/v1/rooms/{id} | PUT | Atualizar |
| /api/v1/rooms/{id} | DELETE | Excluir |

### Tecnologias utilizadas:

- Spring Boot
- Spring Data
- JPA
- H2 Database
- [Lombok](https://projectlombok.org/)
- [Docker](https://docs.docker.com/get-started/)
- Angular 9

### Pré requisito
Para executar este aplicativo, você precisa instalar duas ferramentas: Docker e Docker Compose.

Instruções de como instalar o Docker no [Ubuntu](https://docs.docker.com/engine/install/ubuntu/), [Windows](https://docs.docker.com/docker-for-windows/install/), [Mac](https://docs.docker.com/docker-for-mac/install/).

Docker Compose já está incluído nos pacotes de instalação para Windows e Mac, portanto, apenas usuários do Ubuntu precisam seguir estas [instruções](https://docs.docker.com/compose/install/).

### Executando Prod
Pode ser executado um único comando no terminal:
~~~
$ docker-compose up -d
~~~
Se você quiser pará-lo, execute o seguinte comando:
~~~
$ docker-compose down
~~~

### Executando Dev (localhost)
Pode ser executado um único comando no terminal:
~~~
$ docker-compose adminer up 
~~~

Irá sube duas instâncias do Adminer e do Postgres. O adminer é uma ferramenta para gerenciar conteúdo em bancos de dados Postgres.
A lista completa de endpoints REST disponíveis pode ser encontrada na IU Swagger, que pode ser chamada usando o link: http://localhost:8080/swagger-ui.html

Dentro da pasta do projeto execute o comando no terminal ou na sua IDE de preferencia:

~~~
$ mvn clean spring-boot:run
~~~

Este aplicativo também é colocado no contêiner do Docker e as suas definições podem ser encontrada no arquivo `./Dockerfile`.

@willyms
