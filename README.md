🔢 5-Day Java Project: Number Prediction Challenge
Develop a basic number prediction system that challenges your logical thinking.
---
### Day 1: The First Guess
1.  Create `NumberPredictor.java`.
2.  Generate a random secret number between 1 and 10 (inclusive).
3.  Ask the user: "Guess the secret number (1-10):"
4.  Read their guess.
5.  If the guess matches the secret number, print: "Congratulations! You guessed it!"
6.  Otherwise, print: "Sorry, that's not it. The secret number was [secret number]."

    *Example Output:*
    ```
    Guess the secret number (1-10): 5
    Sorry, that's not it. The secret number was 8.
    ```
---
### Day 2: Smart Feedback
1.  If the guess is incorrect, instead of just saying "that's not it", provide a hint:
    *   If the guess is too high, print: "Too high! The secret number was [secret number]."
    *   If the guess is too low, print: "Too low! The secret number was [secret number]."

    *Example Output:*
    ```
    Guess the secret number (1-10): 7
    Too high! The secret number was 3.
    ```
---
### Day 3: Custom Difficulty Range
1.  Before generating the secret number, ask the user: "Enter the maximum number for the challenge (e.g., 20 for 1-20):"
2.  Generate the secret number using their specified maximum (from 1 to their entered max).
3.  Update the prompt to reflect the new range: "Guess the secret number (1-[user's max]):"

    *Example Output:*
    ```
    Enter the maximum number for the challenge (e.g., 20 for 1-20): 15
    Guess the secret number (1-15): 8
    Too low! The secret number was 12.
    ```
---
### Day 4: Challenge Mode Selector
1.  Reuse Day 3's code.
2.  Before asking for the maximum number, ask the user: "Choose your challenge mode: (E)asy [1-10] or (H)ard [1-50]?"
3.  Based on their input ('E' or 'H'), set the maximum number for the random number generator (10 for Easy, 50 for Hard).
4.  *Do not* ask for a custom maximum if they choose a mode; just use the predefined max.

    *Example Output:*
    ```
    Choose your challenge mode: (E)asy [1-10] or (H)ard [1-50]? E
    Guess the secret number (1-10): 6
    Congratulations! You guessed it!
    ```
---
### Day 5: Review & Repeat Option
1.  After the user makes their guess and receives feedback, *always* display the secret number clearly.
2.  (Open-ended) Add a small feature: Ask the user if they want to play another round. If they type 'Y', your program could print "Starting a new round!" and instruct them to re-run the program. (Since you can't use `while` loops, this is a conceptual "repeat" instruction for the user).
