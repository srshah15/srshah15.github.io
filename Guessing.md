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


