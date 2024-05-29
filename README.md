Aqui está a correção do texto:

---

# apresentacao-desafio-bemol

## Olá, me chamo Theo Trindade e completei o desafio (28/05/2024)

### 🛠️ Ferramentas utilizadas: 

Como deram total liberdade para se utilizar quaisquer ferramentas tanto no Front-end quanto no Back-end, eu resolvi utilizar:

- Back-end: Java com Spring Boot.
- Front-end: Angular 17.

## Guia de como iniciar o projeto:

# Links dos Projetos para clonar:

## Front-end
[https://github.com/theotrin/front-end-bemol](https://github.com/theotrin/front-end-bemol)
[![Copiar](https://img.shields.io/badge/Copiar-%20-%2300cc00)](https://github.com/theotrin/front-end-bemol)

## Back-end
[https://github.com/theotrin/api-todo-bemol](https://github.com/theotrin/api-todo-bemol)
[![Copiar](https://img.shields.io/badge/Copiar-%20-%2300cc00)](https://github.com/theotrin/api-todo-bemol)


Fique tranquilo, vou te mostrar onde apertar e o que fazer para rodar o projeto de maneira simples e fácil!

### 🛠️ Setup de ferramentas: 

Você vai precisar ter instalado no seu computador:
- Java 21
- Angular CLI.

## Setup do Back-end com Java:
![image](https://github.com/theotrin/apresentacao-desafio-bemol/assets/102327842/f4ff6b90-8ec3-4a70-a829-196ef75471a6)

Se você já tiver a versão 21 do Java no seu computador, é simplesmente abrir o IntelliJ, apertar no Play e o servidor estará de pé!

### Endpoints:

### Listar tarefas:
#### `GET` `http://localhost:8080/api/tasks`

#### Exemplo de resposta:
```javascript
// HTTP RESPONSE: 200 OK.
[
  {
    "id": 1,
    "description": "Abrir loja Bemol",
    "completed": true
  },
  {
    "id": 2,
    "description": "Contratar Theo Trindade como estagiário",
    "completed": true
  },
  {
    "id": 3,
    "description": "Checar relatório de vendas",
    "completed": false
  }
]
```
### Adicionar nova tarefa à lista:
#### `POST` `http://localhost:8080/api/tasks`
#### Exemplo de como deve ser enviado o body (em JSON):
```javascript
{
    "description": "Chamar Theo Trindade para fazer parte da equipe" // descrição da nova tarefa
}
```

#### Exemplo de resposta:
```javascript
// HTTP RESPONSE: 201 Created.
```

### Marcar uma tarefa como concluída:
#### `PUT` `http://localhost:8080/api/tasks/id/complete`
Exemplo: 
#### `PUT` `http://localhost:8080/api/tasks/3/complete`

#### Exemplo de resposta:
```javascript
// HTTP RESPONSE: 200 OK.
{
  "id": 2,
  "description": "Contratar Theo Trindade como estagiário",
  "completed": true
}
```
Se você fizer uma nova requisição, a tarefa vai receber o valor contrário do que ela tem no "completed".
### Exemplo
```javascript
// Primeira chamada na API:
{
  "id": 2,
  "description": "Contratar Theo Trindade como estagiário",
  "completed": true // na próxima chamada vai receber o valor false
}
// Segunda chamada na API:
{
  "id": 2,
  "description": "Contratar Theo Trindade como estagiário",
  "completed": false // na próxima chamada vai receber o valor true
}
```
### Deletar uma tarefa da lista:
#### `DELETE` `http://localhost:8080/api/tasks/idDesejado`
Exemplo:
#### `DELETE` `http://localhost:8080/api/tasks/3`

#### Exemplo de resposta:
```javascript
// HTTP RESPONSE: 204 No Content.
```

## Setup do Front-end com Angular:
![image](https://github.com/theotrin/apresentacao-desafio-bemol/assets/102327842/2012e865-271e-4fc1-803d-0ac79afb179a)
- Abrindo o projeto na pasta raiz, basta somente colocar o código `ng serve` e pronto!
- A aplicação deve subir na URL: `http://localhost:4200/`, basta acessar e ver o projeto que deve parecer com isso:

![image](https://github.com/theotrin/apresentacao-desafio-bemol/assets/102327842/307a4bb3-e147-41fc-8d26-539477b812e0)

## Como usar o projeto?

Chegamos na parte mais fácil onde precisamos apenas clicar, então lá vai o guia: 
- Entrando no projeto, você já deve ver as 3 tarefas que sempre subirão quando o projeto for reiniciado.
- Clicando no nome da tarefa, ela deve ficar riscada indicando que foi concluída.
- Apertando no X ao lado, a tarefa deve ser excluída.
- As operações acontecem tanto no Front-end quanto no Back-end.

# 🚀 Diferenciais 🚀 feitos:
## Implementação de testes unitários na API. 
![image](https://github.com/theotrin/apresentacao-desafio-bemol/assets/102327842/ca40fab8-dcdf-470c-8136-21a3173262d0)

- Foram feitos testes unitários utilizando JUnit 5 e Mockito na API.
## Organização de código.
- Busquei organizar o código da maneira mais limpa e organizada possível, sendo fácil de refatorar e entender.
## Responsividade
- Utilizei Bootstrap, que cuida da organização no Front-end, então a aplicação está responsiva em dispositivos móveis também!

# Me chamo Theo Trindade e esse foi meu projeto!
### Estou disponível e entusiasmado para falar sobre ambas as partes do projeto e explicar eventuais blocos de código. Obrigado :D.

