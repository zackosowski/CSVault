#article

*For more info, see the [Unity Manual](https://docs.unity3d.com/Manual/Collider2D.html) article on this component.*

In Unity, colliders are components that define the shape of a [[GameObject]] for the purpose of physical interactions. They are essential for detecting collisions and triggers, allowing developers to implement a wide range of gameplay mechanics, from simple object interactions to complex physics simulations.

----
#### Types of Colliders

Unity offers various types of colliders to suit different needs:

- **Box Collider**: A square shape used for 2D objects. It is efficient for colliding with flat surfaces and box-like structures.
- **Circle Collider**: A circular shape used for 2D objects. Ideal for simulating round objects like balls or planets.
- **Capsule Collider**: A cylindrical shape with semicircular ends, commonly used for character models and humanoid objects.
- **Polygon Collider**: Uses a multi-sided polygon for collision detection, providing precise interactions at the cost of performance.

----
#### Collision Detection

Colliders can trigger different methods, depending on their collision:

- **`OnCollisionEnter()`**: When two colliders intersect, Unity can detect the collision and apply physics responses like bouncing or sliding based on [[Rigidbody]] properties.
- **`OnTriggerEnter()`**: Colliders can be set as triggers, allowing them to detect overlaps without physical reactions. This is useful for events like pickups, zones, or special interactions.

`OnCollisionExit()` and `OnTriggerExit()` are also called when either event happens. All of the above described functions are built into the `MonoBehaviour` class, so you won't have to worry about implementing them.

----
#### Best Practices

- **Use Primitive Colliders When Possible**: Primitive colliders (Box, Circle, Capsule) are more efficient than Polygon Colliders and should be prioritized for performance.
- **Optimize Polygon Colliders**: If using Polygon Colliders, consider simplifying the shape to reduce computational overhead.
- **Layer Management**: Utilize collision layers to manage which objects interact, improving performance and reducing unnecessary calculations.

----
#### Related Articles
[[Component]]
[[Rigidbody]]