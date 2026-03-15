# python-geometry-menu

import math

opcion = 0

while opcion != 10:

    print("\nMENU DE FIGURAS GEOMETRICAS")
    print("1. Rectangulo")
    print("2. Circulo")
    print("3. Trapecio")
    print("4. Paralelogramo")
    print("5. Esfera")
    print("6. Cilindro")
    print("7. Cono")
    print("8. Paralelepipedo")
    print("9. Triangulo Rectangulo")
    print("10. Salir")

    opcion = int(input("Seleccione una opcion: "))

    if opcion == 1:
        base = float(input("Ingrese la base: "))
        altura = float(input("Ingrese la altura: "))
        area = base * altura
        print("El area del rectangulo es:", area)

    elif opcion == 2:
        radio = float(input("Ingrese el radio: "))
        area = math.pi * radio ** 2
        print("El area del circulo es:", area)

    elif opcion == 3:
        base_mayor = float(input("Ingrese la base mayor: "))
        base_menor = float(input("Ingrese la base menor: "))
        altura = float(input("Ingrese la altura: "))
        area = ((base_mayor + base_menor) * altura) / 2
        print("El area del trapecio es:", area)

    elif opcion == 4:
        base = float(input("Ingrese la base: "))
        altura = float(input("Ingrese la altura: "))
        area = base * altura
        print("El area del paralelogramo es:", area)

    elif opcion == 5:
        radio = float(input("Ingrese el radio: "))
        volumen = (4/3) * math.pi * radio ** 3
        print("El volumen de la esfera es:", volumen)

    elif opcion == 6:
        radio = float(input("Ingrese el radio: "))
        altura = float(input("Ingrese la altura: "))
        volumen = math.pi * radio ** 2 * altura
        print("El volumen del cilindro es:", volumen)

    elif opcion == 7:
        radio = float(input("Ingrese el radio: "))
        altura = float(input("Ingrese la altura: "))
        volumen = (math.pi * radio ** 2 * altura) / 3
        print("El volumen del cono es:", volumen)

    elif opcion == 8:
        largo = float(input("Ingrese el largo: "))
        ancho = float(input("Ingrese el ancho: "))
        altura = float(input("Ingrese la altura: "))
        volumen = largo * ancho * altura
        print("El volumen del paralelepipedo es:", volumen)

    elif opcion == 9:
        base = float(input("Ingrese la base: "))
        altura = float(input("Ingrese la altura: "))
        area = (base * altura) / 2
        print("El area del triangulo rectangulo es:", area)

    elif opcion == 10:
        print("Saliendo del programa...")

    else:
        print("Opcion invalida")
