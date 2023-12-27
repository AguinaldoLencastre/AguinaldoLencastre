

Analisa esse que fiz 


agenda_telefonica = {}

def adicionar_contato(nome, numero):
    agenda_telefonica[nome] = numero
    print(f"Contato {nome} adicionado com sucesso!")

def buscar_contato(nome):
    if nome in agenda_telefonica:
        print(f"Nome: {nome}, Número: {agenda_telefonica[nome]}")
    else:
        print(f"Contato {nome} não encontrado na agenda.")

def listar_contatos():
    if agenda_telefonica:
        print("Lista de Contatos:")
        for nome, numero in agenda_telefonica.items():
            print(f"Nome: {nome}, Número: {numero}")
    else:
        print("A agenda telefônica está vazia.")

# Exemplo de uso:
adicionar_contato("Aguinaldo", "123456789")
adicionar_contato("Maria", "933476225")
listar_contatos()
buscar_contato("Aguinaldo")
buscar_contato("Carlos")
