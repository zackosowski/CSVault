#article

Writing a script in [[Unity Game Engine|Unity]] allows developers to create custom [[Component|components]], complete with their own [[Variables|variables]] and [[Functions (C-Sharp)|functions]], that can interact freely with other components. A new script can be created by right clicking an empty space in the Project window, hitting "Create" and pressing the    "[[C-Sharp|C#]] Script" button. After naming the script, the file will be created and the project code will re-compile. An empty script will look something like this:

```c#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class MyScript : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}

```

By default, all Unity components derive from the `MonoBehaviour` class, which offers life-cycle functions for [[GameObject|GameObjects]] such as `Awake()`, `Start()` and `Update()`. Default scripts also have some libraries already imported, including some system libraries needed for some basic functions and the `UnityEngine` library.

---
#### Variables

*Main article: [[Variables]]*

Variables essentially function the same in all programming languages, representing values that can be changed and used in code whenever they need to be. They key difference in declaring C# variables is stating the type of variable. For example, strings must have the `string` keyword, ints must have the `int` keyword, and so on. Here are some examples of C# variable declarations.

```c#
int coins = 457; //creates a `int` variable named coins, default value 457
float health = 13.5f; //`float` variable named health, default 13.5
string name = "Zacc"; //`string` variable named name, default Zacc
```

---
#### Functions

*Main article: [[Functions (C-Sharp)]]*

Functions are large blocks of re-usable code that can be called to execute from within it's own class, or a different class. They are mainly used for full actions or events, such as the player jumping or firing a weapon.

```c#
public void Jump()
{
	//makes the character jump
	rigidBody.AddForce(transform.up * jumpForce);
}
```

---
#### Lists

Main article: [[Lists (C-Sharp)]]

A list is a collection of variables of the same type that can be added to and removed from at any time.

```c#
List<string> fruits = new List<string> { "apple", "banana", "cherry" };

void PrintFruits()
{
	foreach(string fruit in fruits)
	{
		Debug.Log(fruit);
	}
}

//outputs:
//apple
//banana
//cherry
```

----
#### Related Articles
[[Data Types]]
[[Variables]]
[[Lists (C-Sharp)]]
[[Functions (C-Sharp)]]