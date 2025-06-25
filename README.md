# import random

def guess_the_number():
    number_to_guess = random.randint(1, 100)
    print("Welcome to the Guess the Number Game!")
    print("I'm thinking of a number between 1 and 100.")

    while True:
        try:
            guess = int(input("Take a guess: "))
            if guess < number_to_guess:
                print("Too low! Try again.")
            elif guess > number_to_guess:
                print("Too high! Try again.")
            else:
                print("Congratulations! You guessed the number!")
                break
        except ValueError:
            print("Please enter a valid integer.")

if __name__ == "__main__":
    guess_the_number()
    
