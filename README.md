
import random

print("Welcome to the number guessing Game")
secret_number = random.randint(1, 10)
attempt = 0

while True:
    guess = int(input("Enter number between 1 and 10: "))
    attempt += 1

    if guess == secret_number:
        print(f"Correct! You guessed the number in {attempt} tries")
        break
    elif guess > secret_number:
        print("Too high, try again")
    else:
        print("Too low, try again")
