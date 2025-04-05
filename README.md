# 📝 Gerenciador de Tarefas em Python

Este é um projeto simples em Python que permite adicionar, listar, remover e salvar tarefas com prioridade em um arquivo .json. As tarefas são manipuladas por meio de um menu interativo no terminal.

# 📁 Arquivos

tarefas.json: arquivo onde as tarefas são salvas.

main.py: script principal com o código do gerenciador de tarefas.

# 📌 Funcionalidades

## ✅ 1. Adicionar tarefa

O usuário informa o nome e a prioridade da tarefa.

A tarefa é adicionada à lista atual.

## 📋 2. Listar tarefas

Exibe todas as tarefas da lista com o respectivo nome e prioridade.

## 🗑 3. Remover tarefa

O usuário informa o nome da tarefa a ser removida.

Se encontrada, ela é excluída da lista.

## 📅 4. Salvar tarefas

Salva todas as tarefas atuais no arquivo tarefas.json.

## ❌ 5. Sair

Encerra o programa.

## 📂 Estrutura do Código

## 1. Variável de tarefas

tarefas = []

Armazena todas as tarefas em uma lista de dicionários.

## 2. Função salvar_tarefas()

Salva a lista de tarefas no arquivo JSON.

## 3. Função carregar_tarefas()

Carrega tarefas do arquivo JSON se existir, caso contrário inicia uma lista vazia.

## 4. Função adicionar_tarefa(nome, prioridade)

Cria uma nova tarefa e adiciona à lista.

## 5. Função listar_tarefas()

Exibe todas as tarefas no terminal.

## 6. Função remover_tarefas(nome)

Busca a tarefa pelo nome e a remove da lista.

## 7. Laço principal (while True)

Exibe o menu de opções para o usuário interagir com o programa.
