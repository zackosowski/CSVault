#lesson 

#### Targets

- I can create and edit [[GameObject|GameObjects]] using the Scene View, Hierarchy and Inspector windows

- I can add and edit [[Component|components]] to existing GameObjects.

---
#### Lesson

1. Create a new GameObject via the Hierarchy
	1. Right click in an empty spot in the Hierarchy
	2. Navigate to 2D Object > Sprites > Square

2. Manipulate the values of the GameObject's components
	1. Select the new Square object we just created by clicking on it in the Scene View or Hierarchy
	2. In the Inspector Window, change the values of the [[Transform]] component and watch the changes occur on the Scene View
	3. Use widgets and handles in the scene view to manually manipulate the GameObject
	4. When finished, right click the Transform component header and press "Reset" to change all of the variables back to their default values

3. Add a [[Rigidbody|Rigidbody 2D]] component to the object
	1. With the object selected, in the Inspector, click "Add Component"
	2. In the search bar, type "**Rigidbody 2D**"
		- Play the scene to sese the effect this new component has on the Square
		- Try changing the "Gravity Scale" value in the Rigidbody to -1, then re-play the scene

4. Add a [[Collider|Box Collider 2D]] component to the Square

5. Create a platform for the object to fall onto
	1. Duplicate the Square object with "CTRL + D"
	2. Rename the new object to "Platform" and move it to the bottom of the camera view
	3. Stretch the object out by changing the X value in Transform - Scale
	4. Change the Rigidbody - Body Type to Static
	5. Press play and see the new effects


----
#### Assignment

Complete the [[Candy Bowl]] assignment

----
#### Related Articles
[[GameObject]]
[[Component]]