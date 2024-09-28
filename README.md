# Calculadora simple en Python

def suma(a, b):
    return a + b

def resta(a, b):
    return a - b

def multiplicacion(a, b):
    return a * b

def division(a, b):
    if b != 0:
        return a / b
    else:
        return "No se puede dividir entre 0"

def calculadora():
    print("Selecciona la operación:")
    print("1. Suma")
    print("2. Resta")
    print("3. Multiplicación")
    print("4. División")

    eleccion = input("Introduce el número de la operación (1/2/3/4): ")

    num1 = float(input("Introduce el primer número: "))
    num2 = float(input("Introduce el segundo número: "))

    if eleccion == '1':
        print(f"{num1} + {num2} = {suma(num1, num2)}")
    elif eleccion == '2':
        print(f"{num1} - {num2} = {resta(num1, num2)}")
    elif eleccion == '3':
        print(f"{num1} * {num2} = {multiplicacion(num1, num2)}")
    elif eleccion == '4':
        print(f"{num1} / {num2} = {division(num1, num2)}")
    else:
        print("Elección inválida")


calculadora()
