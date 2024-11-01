#assignment

Write a function that lets the player visit a mystic fortune teller who asks for different types of numbers to tell their fortune. Each prompt must be a number of some type, integer or float. If the player enters the wrong type (e.g., a string instead of a number), the program should catch the error and prompt them to try again.

---
#### Overview

1. **Fortune Teller Setup**  
    Introduce the fortune teller, who will ask for different numbers to provide mystical insights.
    
2. **Input Prompts with Type Requirements**  
    The fortune teller asks for the user to input numbers to tell the fortune. You can ask any questions you want for this, but here are some examples:
    - Ask for the player’s **lucky number** (expects an integer).
    - Ask how many **years into the future** they want to see (expects a float).
    - Ask for a **magical multiplier** (expects a float).
    
3. **Error Handling Using try and except**  
    Use try and except to:
    
    - Catch errors if the player inputs the wrong type.
    - Restart the function when an error occurs

1. Read out the fortune  
    Take the input numbers and a random number to calculate the fortune.
---
#### Requirements

| **Less Comfortable** | **More Comfortable** |
| -------------------- | -------------------- |
| 3 inputs             | 5 inputs             |
| 1 randomization      | 1 randomization      |
| 5 possible fortunes  | 10 possible fortunes |

---
#### Hints
Use if/elif/else statements to choose the fortune at the end.

Use [[Operators#Comparison Operators|comparison operators]] to help evaluate the calculated number to choose a fortune.

---
#### How to Submit

Save the file as `fortuneteller.py` in your assignments folder and push your code to your GitHub repository.
