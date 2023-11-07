import random

def forest_adventure():
    print("Welcome to the Forest Adventure!")
    player_name = input("Enter your name: ")
    print(f"Hello, {player_name}! Your journey begins in a dense forest.")

    while True:
        choice = input("Do you want to go left or right? (left/right/quit): ").lower()

        if choice == "left":
            # Generate a random number to represent an encounter
            encounter = random.randint(1, 5)
            if encounter == 1:
                print("You found a treasure chest! You're rich!")
            else:
                print("You encountered a wild beast. Watch out!")
        elif choice == "right":
            # Another random encounter
            encounter = random.randint(1, 5)
            if encounter == 1:
                print("You stumbled upon a hidden pathway.")
            else:
                print("You fell into a pit. Ouch!")
        elif choice == "quit":
            print("Thanks for playing! See you next time.")
            break
        else:
            print("Invalid choice. Please enter 'left', 'right', or 'quit'.")

if __name__ == "__main__":
    forest_adventure()
