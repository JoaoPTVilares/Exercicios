# Exercício: Gestão de Loja de Filmes

## Tema

Desenvolver um programa em C++ para gerir uma pequena loja de filmes. Cada filme tem:

* **Título** (string)
* **Género** (string)
* **Ano de lançamento** (int)
* **Número de cópias disponíveis** (int)

O programa deve permitir ao utilizador gerir os filmes usando um menu.

## Requisitos Funcionais

O programa deve:

1. **Criar dinamicamente** um array de filmes usando memória dinâmica (`new`), começando vazio.
2. Permitir ao utilizador interagir com um menu com as seguintes opções:

   * **Listar filmes**: Mostrar todos os filmes e o número de cópias disponíveis.
   * **Adicionar filme**: Inserir um novo filme, alocando memória dinâmica para ele.
   * **Procurar filme**: Pesquisar filmes pelo título.
   * **Total de cópias**: Calcular o total de cópias de todos os filmes.
   * **Sair**: Liberar toda a memória alocada e terminar o programa.
3. Armazenar os filmes em memória dinâmica, redimensionando o array conforme o utilizador adiciona novos filmes.
4. Garantir que toda a memória alocada é libertada antes do programa terminar.

## Objetivos do Exercício

* Praticar **uso de struct** para armazenar dados.
* Trabalhar com **arrays dinâmicos** e alocação de memória com `new` e `delete`.
* Manipular vetores de structs sem usar `std::vector`.
* Usar estruturas de decisão (`if`, `switch`) e ciclos (`for`, `while`).
* Criar um programa funcional, persistente em memória após a execução.
