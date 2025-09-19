# coding_adventures.py
# A collection of coding adventures, experiments, and learning projects

import random

def hello_world():
    print("👋 Hello, World! The classic first adventure.")

def number_guessing_game():
    print("🎲 Number Guessing Game")
    secret = random.randint(1, 10)
    guess = int(input("Guess a number between 1 and 10: "))
    if guess == secret:
        print("✅ Correct! You guessed it.")
    else:
        print(f"❌ Oops! The number was {secret}.")

def fibonacci(n=10):
    print(f"🔢 First {n} Fibonacci numbers:")
    seq = [0, 1]
    whil len(seq) < n:
        seq.append(seq[-1] + seq[-2])
    print(seq)

    def main(): 
    while True:
        print("\n🚀 Coding Adventures Menu")
        print("1. Hello World")
        print("2. Number Guessing Game")
        print("3. Fibonacci Sequence")
        print("4. Exit")

        choice = input("Choose an adventure (1-4): ")

        if choice == "1":
            hello_world()
        elif choice == "2":
            number_guessing_game()
        elif choice == "3":
            fibonacci()
        elif choice == "4":
            print("Goodbye! Keep coding and exploring. ✨")
            break
        else:
            print("Invalid choice. Try again!")

if __name__ == "__main__":
    main()


