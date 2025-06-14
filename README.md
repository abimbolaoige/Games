# Games
Find here fun games you can play with family and friends 
#### I am putting this codes together, follow for more

### A Simple Letter Guessing Game
``` import random
import string

letter = random.choice(string.ascii_uppercase)

print("Welcome to the Letter Guessing Game!")
print("I'm thinking of a letter between A and Z.")

while True:
    guess = input("Take a guess: ").strip().upper()
    
    if guess < letter:
        print("Too early in the alphabet. Try again.")
    elif guess > letter:
        print("Too late in the alphabet. Try again.")    
    else:
        print("Congratulations! Smart Coder!")
        break
```

### A Simple Number Guessing Game
```
import random
number = random.randint(1,200)

print("Welcome to the number guessing game")
print("I'm thinking of a number between 1 and 200.")

while True:
    guess = int(input("Take a guess: "))

    if guess < number:
        print("Too low. Try again")
    elif guess > number:
        print("Too high. Try again")
    else:
        print("Congratulations, You made it. Agba Coder")
        break
```
### A word or phrase of affection and commendation
```
import random
import difflib

# List of affectionate and commendation words
words_of_affection_and_commendation = [
    'LOVE', 'HUG', 'CARE', 'KISS', 'ADORE', 'CHERISH', 'SACRIFICE',
    'YOU ARE THE BEST', 'I VALUE YOU', 'YOU MAKE ME PROUD',
    'DARLING', 'COMMUNICATION'
]

# Randomly choose a word
word = random.choice(words_of_affection_and_commendation)

print("Welcome to the Word Guessing Game!")
print("I'm thinking of a word or phrase of affection and commendation...")

while True:
    guess = input("Take a guess: ").strip().upper()

    if guess == word:
        print("Congratulations! Smart Coder!")
        break
    else:
       
        close_matches = difflib.get_close_matches(guess, [word], n=1, cutoff=0.6)
        if close_matches:
            print("Too close! Try again.")
        else:
            print("Not close. Try again.")
```

##### Have fun!
