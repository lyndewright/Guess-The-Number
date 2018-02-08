# Guess-The-Number

import random

random_number = random.randint(1,10)


count = 0

while count < 10:
    guess = input("Enter number between 1 and 10 or type 'exit' to quit game.\n")
    if guess.lower() == 'exit':
        break

    guess = int (guess)
    count+=1

    if int (guess) > random_number:
        print ("Too high. Try again or type 'exit' to quit game.")
    elif int (guess) < random_number:
        print ("Too low. Try again or type 'exit' to quit game.")
    elif int (guess) == random_number:
        break
if (guess) == random_number:
    count = str(count)
    print ("You've got it! You've guessed the number in " + (count) + " guesses.")
