#article

*For more info, see the [Unity Manual](https://docs.unity3d.com/ScriptReference/Transform.html) article on this component.*

The Transform [[Component|component]] in [[Unity Game Engine|Unity]] is a fundamental part of the game engine that defines an object's position, rotation, and scale in a 3D or 2D space. Every [[GameObject]] in Unity contains a Transform component, which serves as its primary means of controlling its spatial attributes within the game world.

----
#### Usage

Transform components can be manipulated through the Unity Editor or via scripts using C#. Common operations include moving, rotating, and scaling objects in response to user input or game events. The Transform component of a GameObject can be accessed anytime by [[Script|scripts]] by using the ``transform`` keyword.

----
#### Useful Properties

| **Name**    | **Property Type** | **Is Serialized?** | **Usage**                                                                                                                                        |
| ----------- | ----------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Position    | Vector3           | Yes                | Position of the object in the game world on (x,y,z). 2D Games only use (x,y).                                                                    |
| Rotation    | Vector3           | Yes                | Pitch, yaw and roll of the object (x,y,z). 2D games only use (z).                                                                                |
| Scale       | Vector3           | Yes                | Scale of the object (x,y,z). 2D games only use (x,y).                                                                                            |
| Child Count | int               | No                 | Tracks the number of children the object carries.                                                                                                |
| Parent      | Transform         | No                 | Tracks the parent of an object. Can be `null` if the object has no parent.                                                                       |
| Forward     | Vector3           | No                 | Returns a normalized vector that represents the blue arrow of the transform compass in the world space. Most often used for physics calculations |

----
#### Useful Functions

| **Name**           | Return Type | Parameters         | **Usage**                                                                   |
| ------------------ | ----------- | ------------------ | --------------------------------------------------------------------------- |
| `DetachChildren()` | void        | n/a                | Unparents all children of the Transform                                     |
| `IsChildOf()`      | bool        | Transform `parent` | Checks to see if the GameObject is a child of `parent`.                     |
| `Find()`           | Transform   | string `n`         | Finds a child with the name `n`. Returns `null` if it fails to find a child |
| `Rotate()`         | void        | Vector3 `eulers`   | Rotates the GameObject by the (x,y,z) angles specified in `eulers`.         |

----
#### Hierarchy and Parent-Child Relationships

A GameObject can be the parent or child of another GameObject. When an object is "childed", it mimics changes made to the parent GameObject. For example, moving the parent 3.5 units on the X position will also move the child 3.5 units on the X position.