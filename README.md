import random

def guess_game():
    number = random.randint(1, 100)
    attempts = 0
    print("Guess the number between 1 and 100.")

    while True:
        guess = int(input("Your guess: "))
        attempts += 1
        if guess < number:
            print("Too low! Try again.")
        elif guess > number:
            print("Too high! Try again.")
        else:
            print(f"Correct! You guessed the number in {attempts} attempts.")
            break

guess_game()
