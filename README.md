# Fermi Pico Bagel Game

## Overview

Fermi Pico Bagel is a classic guessing game where the player tries to guess a secret number. The game provides feedback in the form of "Fermi", "Pico", or "Bagel" to help the player get closer to the correct guess.

## Rules

1. The secret number is a string of unique digits.
2. The player inputs their guess.
3. The game provides feedback based on the guess:
   - "Fermi" indicates a correct digit in the correct position.
   - "Pico" indicates a correct digit in the wrong position.
   - "Bagel" indicates no correct digits.
4. The game continues until the player guesses the secret number correctly.

## How to Play

1. Run the game script.
2. Enter your guess when prompted.
3. Receive feedback and continue guessing until you win.

## Example

- Secret number: `123`
- Player's guess: `124`
- Feedback: `Fermi Pico`

## Explanation of Each Step

1. **Store the original number as a string**: The `original_number` is defined as a string.
2. **Take user input**: The program enters an infinite loop to keep asking the user for guesses until they guess correctly.
3. **Check if the number of digits are the same**: The program checks if the length of `guess_number` matches the length of `original_number`. If not, it asks the user for a valid input and continues the loop.
4. **Check for duplicate digits in the guess**: The program uses a `set` to check for duplicate digits in the guess. If there are duplicates, it informs the user and continues the loop.
5. **Check if the guess is correct**: If the guess matches the original number, it prints "Fermi" the correct number of times and breaks the loop, ending the game.
6. **Create an empty list for the output**: An empty list called `output` is created to store the results.
7. **Check for Fermi and Pico**: The program checks each digit in the guess:
   - If a digit is correct and in the correct position, it appends "Fermi" to the output list.
   - If a digit is correct but in the wrong position, it appends "Pico" to the output list.
8. **Create the output string**: The `output_string` is created by joining the `output` list into a string separated by spaces.
9. **Print the result**: The program prints "Bagel" if there are no correct digits; otherwise, it prints the `output_string`.

## Requirements

- Python 3.x

## How to Run

1. Save the code to a file, e.g., `fermi_pico_bagel.py`.
2. Open a terminal or command prompt.
3. Navigate to the directory containing the script.
4. Run the script using the command: `python fermi_pico_bagel.py`.

