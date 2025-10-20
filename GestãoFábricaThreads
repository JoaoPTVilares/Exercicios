# Exercício: Gestão de Fábrica com Produção em Tempo Real

## Tema

Desenvolver um programa em C++ para gerir uma pequena fábrica. Cada produto produzido na fábrica tem:

* **Nome** (string)
* **Categoria** (string)
* **Stock atual** (int)
* **Taxa de produção por hora** (int)

O programa deve simular a produção em tempo real, atualizando o stock automaticamente a cada 5 segundos, enquanto permite que o utilizador interaja com um menu de gestão.

## Objetivos do Exercício

Praticar:

* Uso de **struct** e **vector** para armazenar dados.
* Funções que manipulam vetores de produtos.
* Sincronização de threads com `std::mutex` e `std::thread`.
* Atualização de informação em tempo real no terminal.
* Estruturas de decisão (`if`, `switch`) e ciclos (`for`, `while`).
* Persistência de dados em memória durante a execução.

## Requisitos Funcionais

O programa deve:

* Permitir ao utilizador interagir com um menu que inclui as seguintes opções:

  * **Listar produtos**: Mostrar todos os produtos e o stock atual.
  * **Adicionar produto**: Inserir um novo produto com nome, categoria, stock inicial e taxa de produção.
  * **Procurar produto**: Pesquisar produtos pelo nome.
  * **Total em stock**: Calcular e mostrar o total de unidades em stock de todos os produtos.
  * **Pausar produção**: Interromper temporariamente a produção.
  * **Retomar produção**: Continuar a produção após ter sido pausada.
  * **Visualização em tempo real: Onde a cada 5s o valor do stock aumenta baseado na produção
  * **Sair**: Terminar o programa.

* Iniciar a produção automaticamente ao arrancar o programa, aumentando o stock de cada produto com base na taxa de produção por hora (simulado a cada 5 segundos).

* Exibir um painel de produção em tempo real, atualizando automaticamente o stock de cada produto sem interferir com o menu. O painel deve mostrar:

  * Nome do produto
  * Stock atual
  * Taxa de produção
  * Estado da produção (ON / OFF)

* Garantir que a produção e a atualização do painel são feitas em **threads separadas**, sincronizadas com **mutex** para evitar condições de corrida.

## Requisitos Técnicos

* Utilizar structs, funções, vetores e threads.
* Threads devem ser geridas usando `std::thread` e sincronizadas com `std::mutex`.
* A produção deve poder ser pausada e retomada pelo utilizador a qualquer momento.

## Extras (Opcional)

* Adicionar cores ANSI para o estado da produção (**verde = ON**, **vermelho = OFF**).
* Simular produção proporcional à taxa por hora dividida pelo intervalo de atualização (por exemplo, `taxa/12` a cada 5 segundos).
