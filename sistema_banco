menu = """

[d] Depositar
[s] Sacar
[e] Extrato
[q] Sair

=> """

saldo = 0
limite = 500
extrato = ""
quantidade_saque = 0
QUANTIDADE_LIMITE_SAQUE = 3

while True:

    opcao = input(menu)

    if opcao.lower()== "d":
        DEPOSITO = " DEPÓSITO "
        print("\n" + DEPOSITO.center(41,"="))
        valor = float(input("Informe o valor do depósito: "))

        if valor > 0:
            saldo += valor
            extrato += f"Depósito: R$ {valor:.2f}\n"

        else:
            print("Falha. O valor inserido é inválido.")


    elif opcao.lower() == "s":
        SAQUE = " SAQUE "
        print("\n" + SAQUE.center(41,"="))
        valor = float(input("Informe o valor do saque: "))

        if quantidade_saque >= QUANTIDADE_LIMITE_SAQUE:
            print("\nFalha. Número máximo de saques diário chegou ao limite.")

        elif valor > saldo:
            print("\nFalha. Saldo insuficiente.")

        elif valor > limite:
            print(f"\nFalha. O valor excede o seu limite de R$ {limite:.2f}.")

        elif valor > 0:
            saldo -= valor
            quantidade_saque += 1
            extrato += f"Saque: R$ {valor:.2f}\n"

        else:
            print("Falha. O valor inserido é inválido.")


    elif opcao.lower() == "e":
        SEPARADOR = ""
        EXTRATO = " EXTRATO "
        print("\n" + EXTRATO.center(41, "="))
        print(extrato)
        print(f"\nSaldo: R$ {saldo:.2f}")
        str(print(SEPARADOR.center(41, "=")))


    elif opcao.lower() == "q":
        print("Obrigado por utilizar nossos serviços.")
        break


    else:
        print("Operação inválida, por favor selecione novamente a operação desejada.")
