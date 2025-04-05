
import json

tarefas = []

def salvar_tarefas():
  with open("tarefas.json", "w") as arquivo:
    json.dump(tarefas, arquivo)
  print("Tarefas salvas com sucesso ")

def carregar_tarefas():
  try:
    with open("tarefas.json", "r") as arquivo:
      tarefas = json.load(arquivo)
      print("Tarefas carregadas com sucesso")
      return tarefas
  except:
    print("Nenhuma tarefa encontrada! Começando uma nova lista")
    return []

def adicionar_tarefa( nome, prioridade):
    tarefa = {
        "nome": nome,
        "prioridade": prioridade
      }

    tarefas.append(tarefa)
    print("Tarefa foi adicionada! :", tarefa)

def listar_tarefas():
  print("Tarefas:")
  for tarefa in tarefas:
    print(f"- {tarefa['nome']} (Prioridade{tarefa ['prioridade']})")

def remover_tarefas(nome):
   for tarefa in tarefas:
    if tarefa ['nome'] == nome:
      tarefas.remove(tarefa)
      print("Tarefa removida com sucesso!"  , nome)
      break
    else :
        print("Tarefa não encontrada na lista.")

tarefas = carregar_tarefas()

while True:
    print("** Menu de Opções ** ")
    print("1. Adicionar Tarefa")
    print("2. Listar Tarefas")
    print("3. Remover Tarefas")
    print("4. Salvar tarefas")
    print("5. Sair")
  
    opcao = input("Escolha uma opção: ")
    if opcao == "1": 
      nome = input("Digite o nome Tarefa: ")
      prioridade = input("Digite a prioridade da tarefa ")
      
      adicionar_tarefa(nome, prioridade) 

    elif opcao == "2":
      listar_tarefas()

    elif opcao == "3":
     nome = input("Digite o nome tarefa a ser removida: ")
     remover_tarefas(nome)

    elif opcao == "4":
      salvar_tarefas()

    elif opcao == "5":
      print("Saindo....")
      break 
    else:
      print("Opção inválida. Tente novamente.")
