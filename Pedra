import random

def jogar_pedra_papel_tesoura():
    opcoes = {
        "pedra": 1,
        "papel": 2,
        "tesoura": 3
    }

    opcoes_reverso = {
        1: "Pedra",
        2: "Papel",
        3: "Tesoura"
    }

    while True:
        escolha_usuario_str = input("Escolha Pedra, Papel ou Tesoura: ").lower()
        if escolha_usuario_str in opcoes:
            escolha_usuario = opcoes[escolha_usuario_str]
            break
        else:
            print("Opção inválida. Por favor, escolha Pedra, Papel ou Tesoura.")

    escolha_computador = random.randint(1, 3)

    print(f"Você escolheu: {escolha_usuario_str.capitalize()}")
    print(f"O computador escolheu: {opcoes_reverso[escolha_computador]}")

    if escolha_usuario == escolha_computador:
        print("Resultado: Empatou!")
    elif (
        (escolha_usuario == 1 and escolha_computador == 3) or  # Pedra ganha de Tesoura
        (escolha_usuario == 2 and escolha_computador == 1) or  # Papel ganha de Pedra
        (escolha_usuario == 3 and escolha_computador == 2)     # Tesoura ganha de Papel
    ):
        print("Resultado: Ganhou!")
    else:
        print("Resultado: Perdeu!")

    print(f"O número aleatório gerado pelo computador foi: {escolha_computador}")

if __name__ == "__main__":
    jogar_pedra_papel_tesoura()
