import random

def jugar_adivinanza():
    numero_secreto = random.randint(1, 10)
    intentos = 0

    print("¡Bienvenido al juego de adivinanzas!")
    print("Estoy pensando en un número del 1 al 10")

    while True:
        intento = int(input("Tu adivinanza: "))
        intentos += 1

        if intento == numero_secreto:
            print(f"¡Correcto! Has adivinado en {intentos} intentos.")
            break
        else:
            print("Incorrecto. ¡Inténtalo de nuevo!")

if __name__ == "__main__":
    jugar_adivinanza()
--->
