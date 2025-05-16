# TheSims
Criando uma lista

personagens = []

while True:
    nome = input("\nNome do personagem (ou 'sair' para encerrar): ")
    if nome.lower() == 'sair':
        break

    idade = input("Idade do personagem: ")
    traço = input("Traço de personalidade: ")

    personagem = {
        "Nome": nome,
        "Idade": idade,
        "Traço": traço
    }

    personagens.append(personagem)

    print("\nPersonagens novos:")
for personagem in personagens:
    print(f"Nome: {personagem´['Nome]}, Idade: {personagem['Idade]}, Traço: {personagem['Traço]}")
