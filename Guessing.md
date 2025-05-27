# Random Guessing Game Flowchart

```mermaid
flowchart TD
    A[Start] --> B[Generate random number between 1 and 100]
    B --> C[Prompt user to enter a guess]
    C --> D{Is input a number?}
    D -- No --> E[Display error message and re-prompt]
    E --> C
    D -- Yes --> F{Is guess = target number?}
    F -- Yes --> G[Display 'Correct!' message]
    G --> H[End]
    F -- No --> I{Is guess > target number?}
    I -- Yes --> J[Display 'Too high' message]
    I -- No --> K[Display 'Too low' message]
    J --> C
    K --> C


1. Start
The program begins execution.

2. Generate Random Number
The computer randomly selects a number between 1 and 100. This is the number the user must guess.

3. Prompt for Guess
The user is prompted to enter a guess.

4. Input Validation
The program checks whether the user entered a valid number:

If not a number: Show an error message and ask the user to try again.

If it is a number: Proceed to evaluate the guess.

5. Check Guess
If the guess equals the target number: Display a “Correct!” message and end the program.

If the guess is greater than the target: Display a “Too high” message.

If the guess is less than the target: Display a “Too low” message.

6. Repeat Loop
If the guess is incorrect, return to prompting the user for a new guess. This loop continues until the correct number is guessed.

7. End
Once the correct number is guessed, the game ends.

