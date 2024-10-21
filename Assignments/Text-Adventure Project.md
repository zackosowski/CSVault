The **Text-Adventure Project** is a creative assignment designed to reinforce programming concepts while allowing you to build your own interactive text-based game. Through this project, you will craft a world filled with choices and outcomes, applying your knowledge of functions, conditionals, and basic game logic to deliver a dynamic and engaging experience for players.

---
#### Overview

In a **text-adventure game**, players progress through a series of story-driven encounters by making choices at key moments. The outcome of each decision changes the flow of the game, making every playthrough potentially unique. You will design your own adventure, using Python to write the game's logic and structure. The game will consist of multiple interconnected encounters, where the player can make choices that impact the storyline.

The final product will be a fully functional text-adventure game that engages players with a series of narrative challenges and decisions.

#### Project Requirements

1. **Game Structure**: 
   - The game should consist of at least 20 different **encounters**, each represented by its own function.
   - An encounter only counts towards the requirement if the player can make a decision that influences the game's outcome in some way (e.g., choosing a path, solving a puzzle, or interacting with a character).
   
2. **Player Choices**:
   - Each encounter should present the player with multiple options, and their choices must lead to different outcomes or scenarios within the game.
   
3. **Game Flow**:
   - The encounters should be logically connected, with some decisions leading to additional encounters or influencing later stages of the game.

4. **Code Organization**:
   - Encounters must be organized into separate functions. This not only keeps the code clean but allows for easy updates and modifications to individual sections of the game.

5. **Ending**: 
   - The game should have at least five distinct endings, determined by the player's choices throughout the adventure.
   
---
#### Example

Here’s a simple example of how a text-adventure game might start:

```python
def start_adventure():
    print("You stand at the entrance of a dark forest. Do you:")
    print("1. Enter the forest")
    print("2. Turn back and go home")
    
    choice = input("> ")
    
    if choice == "1":
        enter_forest()
    elif choice == "2":
        go_home()
    else:
        print("Invalid choice. Try again.")
        start_adventure()

def enter_forest():
    print("You bravely step into the forest and hear strange noises...")
    # More encounters and choices follow

def go_home():
    print("You decide it's safer at home, but your adventure ends here.")
    # End of the game or new encounters
```

Each encounter, such as "enter_forest()" or "go_home()", would represent a unique situation that allows the player to make decisions. The story can branch in numerous directions based on the choices made.

---
#### Hints and Tips

- **Start small**: Focus on getting a few encounters working first before expanding your game. You can always build on your foundation later.

- **Use conditionals effectively**: Make use of `if`, `elif`, and `else` statements to guide the player's choices.

- **Test each function**: As you develop, test your encounters one at a time to ensure each part works as expected.

- **Branching paths**: Think creatively about how choices can lead to different encounters. For example, a choice made early in the game might influence what happens later.

- **Variable tracking**: Consider using variables to keep track of important information, such as whether the player has found a key or completed a quest. Read [[scope]] to review global vs local variables
  
---
### Grading and Rubric

The **Text-Adventure Project** is worth a total of **50 points** and counts as the Unit 3 Test. Below is the grading rubric, which outlines how points will be awarded across various aspects of the project.

###### Rubric

| **Category**                        | **Points** | **Description**                                                                                                                                 |
| ----------------------------------- | ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **Encounters (20 total)**           | 40 points  | Each encounter is worth up to 2 points: 1 point if the encounter exists, and 1 point if it functions correctly without bugs.                    |
| **Code Organization and Structure** | 5 points   | The code is well-organized, with each encounter in its own function. Variables and functions are clearly named, and the code is easy to follow. |
| **Endings and Game Completion**     | 5 points   | One point for each distinct ending (five total).                                                                                                |

###### Point Breakdown:

1. **Encounters (40 points total)**:
   - Each of the 20 required encounters is worth up tp 2 points each:
     - **1 point** if the encounter exists.
     - **1 point** if the encounter works correctly and is free of bugs.
   - Encounters that do not exist or do not work as expected will earn 0 points for that section.

2. **Code Organization and Structure (5 points)**:
   - Full points are awarded if the code is clean, well-organized, commented well, and easy to read, with each encounter in its own function.
   - Partial points for disorganized or difficult-to-follow code.
   - Zero points for chaotic, poorly organized code that is "unreadable".

3. **Endings and Game Completion (5 points)**:
   - One point for each different ending. 
   - Each ending must be unique to count towards the five. Reaching a "You Died!" ending in five different places only counts as one ending.

###### Late Submissions:
- **Late submissions** will receive a **Two point deduction** for each day late, up to a maximum of 20 points.

---
#### How to Submit

Create a file in your tests folder called `textadventure.py` and push your changes to Github.