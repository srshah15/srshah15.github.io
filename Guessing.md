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


Description:

Start: The program begins execution.

Generate Random Number: A random number is selected between 1 and 100. This will be the target the user tries to guess.

User Prompt: The user is asked to enter their guess.

Input Validation: The program checks if the user’s input is a valid number:

If not a number, the user is shown an error and asked to try again.
If a valid number, proceed to checking the guess.

Guess Evaluation:

If the guess is equal to the target number, display a "Correct!" message and end the program.
If the guess is greater than the target, display "Too high".
If the guess is less than the target, display "Too low".

Repeat Guessing Loop: If the guess is incorrect, the user is re-prompted to guess again. The loop continues until the correct number is guessed.

End: The game concludes once the correct number has been guessed.

