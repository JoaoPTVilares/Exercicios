# Projeto: API REST em C++

## Descrição
O objetivo deste projeto é criar uma **API REST** em **C++** que realize as operações de **CRUD** (Create, Read, Update, Delete) sobre um conjunto de **Colaboradores**.  

Podem utilizar **as bibliotecas que preferirem** (por exemplo: [CppRestSDK](https://github.com/microsoft/cpprestsdk), [Crow](https://crowcpp.org/), [Drogon](https://github.com/drogonframework/drogon), entre outras).

---

## Requisitos Funcionais

### Endpoints

#### **GET /colaboradores**
- Retorna uma lista em **JSON** com todos os colaboradores.
- **Resposta (200 OK):**
  ```json
  [
    {
      "id": 1,
      "nome": "João Silva",
      "morada": "Rua das Flores 123",
      "data_nascimento": "1990-05-10",
      "departamento": "Recursos Humanos"
    },
    ...
  ]
GET /colaboradores/{id}

Retorna o colaborador correspondente ao id especificado.

Resposta (200 OK):

{
  "id": 1,
  "nome": "João Silva",
  "morada": "Rua das Flores 123",
  "data_nascimento": "1990-05-10",
  "departamento": "Recursos Humanos"
}


Erro (404 Not Found):

{ "erro": "Colaborador não encontrado." }

POST /colaboradores

Cria um novo colaborador a partir de um objeto JSON enviado no corpo da requisição.

Exemplo de corpo:

{
  "nome": "Maria Costa",
  "morada": "Avenida Central 45",
  "data_nascimento": "1988-09-21",
  "departamento": "Financeiro"
}


Resposta (201 Created):

{ "mensagem": "Colaborador criado com sucesso.", "id": 2 }

PATCH /colaboradores/{id}

Atualiza um ou mais campos do colaborador com o id especificado.

Exemplo de corpo:

{
  "departamento": "Marketing"
}


Resposta (200 OK):

{ "mensagem": "Colaborador atualizado com sucesso." }


Erro (404 Not Found):

{ "erro": "Colaborador não encontrado." }

DELETE /colaboradores/{id}

Remove o colaborador correspondente ao id.

Resposta (200 OK):

{ "mensagem": "Colaborador removido com sucesso." }

Erro (404 Not Found):

{ "erro": "Colaborador não encontrado." }

Persistência de Dados

A aplicação deve garantir persistência da informação, gravando os dados dos colaboradores em ficheiros locais (o formato é de livre escolha, por exemplo: JSON, CSV, binário, etc.).

Estrutura do Objeto Colaborador
Campo	Tipo	Descrição
nome	string	Nome completo do colaborador
morada	string	Endereço do colaborador
data_nascimento	string	Data de nascimento (YYYY-MM-DD)
departamento	string	Departamento em que trabalha


Sugestões de Bibliotecas

Drogon Framework
 — moderno e rápido.

Crow
 — leve e simples.

CppRestSDK
 — da Microsoft, bem documentado.
