#article 

*For additional information, see the [Unity Manual](https://docs.unity3d.com/Manual/class-Rigidbody2D.html) page on this topic.*

In [[Unity Game Engine|Unity]], a Rigidbody is a [[Component|component]] that enables an object to be influenced by physics. By adding a Rigidbody to a [[GameObject]], developers can simulate realistic movements and interactions within a 3D or 2D environment, allowing for behaviors such as gravity, collisions, and other forces.

----
#### Key Features

- **Physics Simulation**: Rigidbodies utilize Unity's physics engine to simulate forces and interactions. They can respond to gravity, drag, and other forces, making them ideal for dynamic objects in a game.

- **Mass and Drag**: Each Rigidbody can be assigned a mass, affecting how it reacts to forces. Drag can also be applied to control how quickly an object slows down when moving through space.

- **Kinematic Rigidbodies**: Developers can set Rigidbodies to be kinematic, which means they will not be affected by physics forces but can still influence other objects. This is useful for objects that need to move in a predetermined way, such as platforms or vehicles.

- **Collisions**: Rigidbodies work with colliders to manage interactions with other GameObjects. They detect collisions and triggers, enabling a variety of gameplay mechanics, from simple interactions to complex physics puzzles.

- **Scripting and Control**: Rigidbodies can be manipulated through scripts, allowing developers to apply forces, set velocities, or trigger interactions programmatically. The Rigidbody API provides functions for adding forces, setting constraints, and controlling movement.

----
#### Types of Rigidbodies

1. **3D Rigidbodies**: Used for three-dimensional game objects. They can rotate and move in three-dimensional space.
2. **2D Rigidbodies**: Designed for 2D games, these Rigidbodies use a simplified physics model and are optimized for 2D environments.

----
#### Best Practices

- Use Rigidbodies for objects that require realistic physical interactions, such as characters, projectiles, and environmental elements.
- Avoid unnecessary Rigidbodies on static objects, as this can lead to performance issues.
- Optimize performance by adjusting collision detection settings and using layers to manage interactions.