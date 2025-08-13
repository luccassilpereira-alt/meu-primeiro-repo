# meu-primeiro-repo
def soma(a, b):
    return a + b

def subtracao(a, b):
    return a - b

def multiplicacao(a, b):
    return a * b

def divisao(a, b):
    if b == 0:
        return "Erro: divisão por zero!"
    return a / b

print("=== Calculadora Simples ===")
print("Operações disponíveis: +, -, *, /")

while True:
    op = input("\nEscolha uma operação (+, -, *, /) ou 'sair' para encerrar: ")

    if op.lower() == 'sair':
        print("Encerrando a calculadora. Até mais!")
        break

    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))

    if op == '+':
        print(f"Resultado: {soma(num1, num2)}")
    elif op == '-':
        print(f"Resultado: {subtracao(num1, num2)}")
    elif op == '*':
        print(f"Resultado: {multiplicacao(num1, num2)}")
    elif op == '/':
        print(f"Resultado: {divisao(num1, num2)}")
    else:
        print("Operação inválida!")
