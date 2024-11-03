#lesson 

#### Targets

- I can create and add a script to an existing [[GameObject]]

- I can use a custom script to manipulate the [[Component|components]] of a GameObject

---
#### Lesson

1. Create a new script in the Project window
	- Right click > Create > C# Script
	- Name this new script `ObjectExploder` and open it

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
		 - Test the new code
	3. Prepare our variables
		- Create a new `float` variable named `explosionForce` with the default value set to 100.
		- Another `float`, this time with the name `explosionRadius` and default value of 2.
	4. Push all nearby objects away
		- In `Explosde()`, create new temporary array and add all of the nearby GameObjects to it using `Physics2D.OverlapCircle()`. Use the `explosionRadius` we created earlier.
		- Create a `foreach` loop to iterate through all of the `Collider2D`s in your list.
		- Determine the direction the push force should be applied in by subtracting the pushed Objects position from this Objects position, then normalizing it.
		- Get the [[Rigidbody|Rigidbody2D]] component from the Collider, and add the force. Use the `explodeForce` we created earlier.

Make sure the `ObjectExploder` is attached to all of your Candy objects. If done correctly, the final product should look something like this:

![[ObjectExploderExample.gif]]

----
#### Final Script

```c#
float explodeForce = 25f;
float explosionRadius = 2f;
private void OnMouseDown()
{
    Explode();
}

void Explode()
{
    //get all nearby Collider2Ds via radius
    Collider2D[] nearbyColliders = Physics2D.OverlapCircleAll(transform.position, explosionRadius);

    //iterate through each Collider2D in range
    foreach (Collider2D obj in nearbyColliders)
    {
        //determine the direction to add the force in
        Vector2 dir = (obj.transform.position - transform.position).normalized;

        //add the force to the GameObject
        obj.GetComponent<Rigidbody2D>().AddForce(dir * explodeForce, ForceMode2D.Impulse);
    }

    //when finished, destroy this GameObject
    Destroy(gameObject);
}
```