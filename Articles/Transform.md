#article

 *For more info, see the [Unity Manual](https://docs.unity3d.com/ScriptReference/Transform.html) article on this component.*

The Transform [[Component|component]] in [[Unity Game Engine|Unity]] is a fundamental part of the game engine that defines an object's position, rotation, and scale in a 3D or 2D space. Every [[GameObject]] in Unity contains a Transform component, which serves as its primary means of controlling its spatial attributes within the game world.

![[TransformDefault.png]]

----
#### Usage

Transform components can be manipulated through the Unity Editor or via scripts using C#. Common operations include moving, rotating, and scaling objects in response to user input or game events. Since it is an inherited component attached to all GameObjects, the Transform component can be accessed anytime by [[Scripting in Unity|scripts]] by using the ``transform`` keyword.

----
#### Useful Properties

| **Name**     | **Property Type** | **Is Serialized?** | **Usage**                                                                                                                                        |
| ------------ | ----------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| `position`   | Vector3           | Yes                | Position of the object in the game world on (x,y,z). 2D Games only use (x,y).                                                                    |
| `rotation`   | Vector3           | Yes                | Pitch, yaw and roll of the object (x,y,z). 2D games only use (z).                                                                                |
| `scale`      | Vector3           | Yes                | Scale of the object (x,y,z). 2D games only use (x,y).                                                                                            |
| `childCount` | int               | No                 | Tracks the number of children the object carries.                                                                                                |
| `parent`     | Transform         | No                 | Tracks the parent of an object. Can be `null` if the object has no parent.                                                                       |
| `up`         | Vector2           | No                 | Returns a normalized vector that represents the green arrow of the transform compass in the scene view. Most often used for physics calculations |
| `right`      | Vector2           | No                 | Returns a normalized vector that represents the red arrow of the transform compass in the scene view. Most often used for physics calculations   |

----
#### Useful Functions

| **Name**           | Return Type | Parameters         | **Usage**                                                                                    |
| ------------------ | ----------- | ------------------ | -------------------------------------------------------------------------------------------- |
| `DetachChildren()` | void        | n/a                | Unparents all children of the Transform                                                      |
| `IsChildOf()`      | bool        | Transform `parent` | Checks to see if the GameObject is a child of `parent`.                                      |
| `Find()`           | Transform   | string `n`         | Returns the first listed child with the name `n`. Returns `null` if it fails to find a child |
| `Rotate()`         | void        | Vector3 `eulers`   | Rotates the GameObject by the (x,y,z) angles specified in `eulers`.                          |

----
#### Hierarchy and Parent-Child Relationships

A GameObject can be the parent or child of another GameObject. When an object is "childed", it mimics changes made to the parent GameObject's transform. For example, moving the parent 3.5 units on the X axis will also move the child 3.5 units on the X axis.