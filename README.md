# Task Management Application

Este é um projeto de gerenciamento de tarefas desenvolvido em Java utilizando o framework Spring Boot. A aplicação permite criar, atualizar, visualizar e excluir tarefas.

## Pré-requisitos

Certifique-se de ter os seguintes softwares instalados em seu ambiente de desenvolvimento:

- JDK 17 ou superior
- Maven 3.6.0 ou superior
- Git (opcional)

## Clonando o Repositório

Se você ainda não clonou o repositório, use o seguinte comando:

```bash
git clone https://github.com/TcheloBorgas/Java_Sem.git
git clone https://github.com/TcheloBorgas/task-management-frontend.git
```

# Estrutura do Projeto
A estrutura do projeto é a seguinte:

taskmanagement/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           └── taskmanagement/
│   │   │               ├── controller/
│   │   │               │   └── TaskController.java
│   │   │               ├── model/
│   │   │               │   └── Task.java
│   │   │               └── service/
│   │   │                   └── TaskService.java
│   │   └── resources/
│   │       └── application.properties
│   └── test/
│       └── java/
│           └── com/
│               └── example/
│                   └── taskmanagement/
│                       └── TaskmanagementApplicationTests.java
├── .gitignore
├── mvnw
├── mvnw.cmd
├── pom.xml
└── README.md


# Executando a Aplicação
## Usando o Maven
Para compilar e executar a aplicação, siga os passos abaixo:

Limpar o projeto:

```bash
mvn clean
```

Instalar as dependências:


```bash
mvn install
```


Executar a aplicação:

```bash
mvn spring-boot:run
```


# Usando o IDE
Se você estiver usando uma IDE como IntelliJ IDEA ou Eclipse, siga estes passos:

1. Importe o projeto como um projeto Maven existente.
2. Aguarde a IDE baixar todas as dependências.
3. Navegue até a classe TaskmanagementApplication e execute-a como uma aplicação Java.

# Endpoints Disponíveis
A aplicação possui os seguintes endpoints:

* GET /tasks: Retorna todas as tarefas.
* GET /tasks/{id}: Retorna uma tarefa específica pelo ID.
* POST /tasks: Cria uma nova tarefa.
* PUT /tasks/{id}: Atualiza uma tarefa existente pelo ID.
* DELETE /tasks/{id}: Exclui uma tarefa pelo ID.

# Estrutura do Código
## Task
A classe Task representa o modelo de dados da aplicação. Está anotada com @Entity e contém os seguintes campos:

* id: Identificador único da tarefa.
* title: Título da tarefa.
* description: Descrição da tarefa.

## TaskController
A classe TaskController é responsável por lidar com as requisições HTTP. Contém os métodos para cada endpoint da aplicação.

## TaskService
A classe TaskService contém a lógica de negócios da aplicação. É responsável por interagir com o repositório de dados e fornecer os métodos necessários para o controlador.

## Testes
Os testes estão localizados no pacote src/test/java e utilizam o framework JUnit para testes unitários e de integração. Para executar os testes, use o comando:

```bash
mvn test
```


# Problemas Comuns
## Erro de Versão de Arquivo de Classe
Se você encontrar um erro indicando uma versão de arquivo de classe não suportada, certifique-se de que está usando a versão correta do JDK configurada no pom.xml.

## Dependências Faltando
Se houver erros de compilação indicando pacotes ausentes, verifique se todas as dependências estão corretamente especificadas no arquivo pom.xml.

# Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

# Licença
Este projeto está licenciado sob a licença MIT - veja o arquivo LICENSE para mais detalhes