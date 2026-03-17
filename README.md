pi = 3.1416
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

    try:
        opcion = int(input("Seleccione una opcion: "))
    except ValueError:
        print("Ingrese un numero valido")
        continue

    if opcion == 1:

        base = -1
        while base <= 0:
            try:
                base = float(input("Ingrese la base: "))
                if base <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                base = -1

        altura = -1
        while altura <= 0:
            try:
                altura = float(input("Ingrese la altura: "))
                if altura <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                altura = -1

        area = base * altura
        print("El area del rectangulo es:", area)

    elif opcion == 2:

        radio = -1
        while radio <= 0:
            try:
                radio = float(input("Ingrese el radio: "))
                if radio <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                radio = -1

        area = pi * radio ** 2
        print("El area del circulo es:", area)

    elif opcion == 3:

        base_mayor = -1
        while base_mayor <= 0:
            try:
                base_mayor = float(input("Ingrese la base mayor: "))
                if base_mayor <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                base_mayor = -1

        base_menor = -1
        while base_menor <= 0:
            try:
                base_menor = float(input("Ingrese la base menor: "))
                if base_menor <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                base_menor = -1

        altura = -1
        while altura <= 0:
            try:
                altura = float(input("Ingrese la altura: "))
                if altura <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                altura = -1

        area = ((base_mayor + base_menor) * altura) / 2
        print("El area del trapecio es:", area)

    elif opcion == 4:

        base = -1
        while base <= 0:
            try:
                base = float(input("Ingrese la base: "))
                if base <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                base = -1

        altura = -1
        while altura <= 0:
            try:
                altura = float(input("Ingrese la altura: "))
                if altura <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                altura = -1

        area = base * altura
        print("El area del paralelogramo es:", area)

    elif opcion == 5:

        radio = -1
        while radio <= 0:
            try:
                radio = float(input("Ingrese el radio: "))
                if radio <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                radio = -1

        volumen = (4/3) * pi * radio ** 3
        print("El volumen de la esfera es:", volumen)

    elif opcion == 6:

        radio = -1
        while radio <= 0:
            try:
                radio = float(input("Ingrese el radio: "))
                if radio <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                radio = -1

        altura = -1
        while altura <= 0:
            try:
                altura = float(input("Ingrese la altura: "))
                if altura <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                altura = -1

        volumen = pi * radio ** 2 * altura
        print("El volumen del cilindro es:", volumen)

    elif opcion == 7:

        radio = -1
        while radio <= 0:
            try:
                radio = float(input("Ingrese el radio: "))
                if radio <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                radio = -1

        altura = -1
        while altura <= 0:
            try:
                altura = float(input("Ingrese la altura: "))
                if altura <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                altura = -1

        volumen = (pi * radio ** 2 * altura) / 3
        print("El volumen del cono es:", volumen)

    elif opcion == 8:

        largo = -1
        while largo <= 0:
            try:
                largo = float(input("Ingrese el largo: "))
                if largo <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                largo = -1

        ancho = -1
        while ancho <= 0:
            try:
                ancho = float(input("Ingrese el ancho: "))
                if ancho <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                ancho = -1

        altura = -1
        while altura <= 0:
            try:
                altura = float(input("Ingrese la altura: "))
                if altura <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                altura = -1

        volumen = largo * ancho * altura
        print("El volumen del paralelepipedo es:", volumen)

    elif opcion == 9:

        base = -1
        while base <= 0:
            try:
                base = float(input("Ingrese la base: "))
                if base <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                base = -1

        altura = -1
        while altura <= 0:
            try:
                altura = float(input("Ingrese la altura: "))
                if altura <= 0:
                    print("Ingrese un numero valido")
            except ValueError:
                print("Ingrese un numero valido")
                altura = -1

        area = (base * altura) / 2
        print("El area del triangulo rectangulo es:", area)

    elif opcion == 10:
        print("Saliendo del programa...")

    else:
        print("Opcion invalida")
