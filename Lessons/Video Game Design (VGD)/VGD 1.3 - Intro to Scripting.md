#lesson 

#### Targets

- I can create and add a script to an existing [[GameObject]]

- I can use a custom script to manipulate the [[Component|components]] of a GameObject

---
#### Lesson

1. Create a new script in the Project window
	- Right click > Create > C# Script
	- Name this new script "ObjectExploder" and open it

2. Review [[Scripting in Unity]] together as a class

3. Write our "ObjectExploder" script
	1. Detect when the player clicks on the GameObject
		- Add the `OnMouseDown()` function
			- This function will activate whenever the player clicks within the GameObject's [[Collider|collider]]
		- Write a `Debug.Log()` message in the new function
		- Test the code and note the message in the console
	2. Remove the GameObject from the scene
		 - Create a new function named `Explode()`
		 - Call `Destroy(gameObject)` in the function
		 - Call `Explode()` in `OnMouseDown()`
		 - 