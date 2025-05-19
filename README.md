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
while True:
    excluir = input("\nDeseja excluir algum personagem? (s/n): ").lower()
    if excluir == 's':
        try:
            indice = int(input("Digite o número do personagem que deseja excluir: "))
            if 0 <= indice < len(personagens):
                removido = personagens.pop(indice)
                print(f"Personagem '{removido['Nome']}' removido.")
        
        except ValueError:
            print("Por favor, digite um número válido.")
    elif excluir == 'n':
        break
    else:
        print("Digite 's' para sim ou 'n' para não.")

print("\nLista final de personagens:")
for personagem in personagens:
    print(f"Nome: {personagem['Nome']}, Idade: {personagem['Idade']}, Traço: {personagem['Traço']}")
