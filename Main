import random

def play():
    user = input("Escolha um: 'r' para Pedra, 'p' para Papel, 't' para Tesoura.\n")
    computer = random.choice(['r', 'p', 't'])

    print(f"O jogador 2 escolheu: {traduz(computer)}")


    if user == computer:
        print(f"Você escolheu {traduz(user)}, jogador 2 tambem escolheu {traduz(computer)}")
        return 'Empate!'

    if venceu(user, computer):
        print(f"Você escolheu {traduz(user)}, {traduz(user)} vence {traduz(computer)}")
        return 'Você venceu!!'

    print(f"Você escolheu {traduz(user)}, {traduz(user)} perde para {traduz(computer)}")
    return 'Você perdeu HAHAHA'

def venceu(jogador1, jogador2):
    if (jogador1 == 'r' and jogador2 == 't') or \
       (jogador1 == 't' and jogador2 == 'p') or \
       (jogador1 == 'p' and jogador2 == 'r'):
        return True
    return False

def traduz(letra):
    if letra == 'r':
        return 'Pedra'
    elif letra == 'p':
        return 'Papel'
    elif letra == 't':
        return 'Tesoura'
    else:
        return 'Desconhecido'

print(play())
