#article

In [[Unity Game Engine|Unity]], a component is a fundamental building block that defines the behavior, appearance, and functionality of [[GameObject|GameObjects]]; they are essentially the life-blood of the engine and all games created with it. Unity's component-based architecture allows developers to create complex game elements by combining various components, facilitating modular design and reusability.

----
#### Component Types

There are a large number of different component types and those that come pre-packaged with the engine, and are essential to create any type of game. They include, but are not limited to:

| **Name of Component**                | **Comes with Unity?** | **Usage**                                                                                                                                                                    |
| ------------------------------------ | --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [[Transform]]                        | Yes                   | Component that is essential for all GameObjects. Keeps track of the objects position, rotation and scale.                                                                    |
| [[Sprite Renderer]]                  | Yes                   | Used to apply [[Sprite\|sprites]] to GameObjects, allowing them to be visible in the Scene and Game Views                                                                    |
| [[Character Controller]]             | Only 3D controller    | Gives players the ability to take control of a game object, move around and interact with the game world.                                                                    |
| [[Rigidbody]]                        | Yes                   | Used to simulate physics on the applied GameObject. Used in tandem with [[Collider\|colliders]].                                                                             |
| [[Collider]]                         | Yes                   | Allows a GameObject with the Rigidbody component to interact with other Rigidbodies.                                                                                         |
| [[Unity Animation System\|Animator]] | Yes                   | Allows automatic manipulation of a GameObject's component variables through the use of animations. Most often used to animate Sprite Renderers or different parts of a mesh. |

----
#### Creating and Using Components

Components can be created and assigned to GameObjects through the Unity Editor. Developers can either use pre-existing components or [[Scripting in Unity|write custom scripts]] to extend functionality. Custom components allow for specific behaviors tailored to the needs of the game.

**Best Practices**

- **Reuse Components**: Use shared components to reduce redundancy and improve project organization.
- **Keep Components Focused**: Aim for single-responsibility components, which simplifies debugging and enhances maintainability.
- **Performance Considerations**: Be mindful of component usage, as excessive or inefficient components can impact game performance.