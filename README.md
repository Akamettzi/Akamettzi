import random

def guess_the_number():
    number = random.randint(1, 100)
    attempts = 0

    print("Bienvenue dans 'Devine le nombre' !")
    print("Je pense à un nombre entre 1 et 100.")

    while True:
        guess = int(input("Devine le nombre : "))
        attempts += 1

        if guess < number:
            print("Trop bas. Essaye encore.")
        elif guess > number:
            print("Trop haut. Essaye encore.")
        else:
            print(f"Bravo ! Tu as deviné le nombre en {attempts} essais.")
            break

guess_the_number()

