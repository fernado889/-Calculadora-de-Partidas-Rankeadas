# -Calculadora-de-Partidas-Rankeadas
def calcula_rankeada(vitorias, derrotas):
    saldo_vitorias = vitorias - derrotas
    if vitorias < 10:
        nivel = "Ferro"
    elif 11 <= vitorias <= 20:
        nivel = "Bronze"
    elif 21 <= vitorias <= 50:
        nivel = "Prata"
    elif 51 <= vitorias <= 80:
        nivel = "Ouro"
    elif 81 <= vitorias <= 90:
        nivel = "Diamante"
    elif 91 <= vitorias <= 100:
        nivel = "Lendário"
    else:
        nivel = "Imortal"
    
    return f"O Herói tem de saldo de {saldo_vitorias} está no nível de {nivel}"
    print(calcula_rankeada(15, 5))  # Output: O Herói tem de saldo de 10 está no nível de Bronze
print(calcula_rankeada(60, 20))  # Output: O Herói tem de saldo de 40 está no nível de Ouro
