#article

*For additional information, see the [Unity Manual](https://docs.unity3d.com/ScriptReference/Transform.html) page on this topic.*

The Transform [[Component|component]] in [[Unity Game Engine|Unity]] is a fundamental part of the game engine that defines an object's position, rotation, and scale in a 3D or 2D space. Every [[GameObject]] in Unity contains a Transform component, which serves as its primary means of controlling its spatial attributes within the game world.

----
#### Key Properties

 1. Position
	 - The Position property determines the object's location in the game world, specified in world or local coordinates. It is represented as a vector (x, y, z) for 3D objects and (x, y) for 2D objects.

 2. Rotation
	 - The Rotation property defines the object's orientation. In Unity, rotation can be represented using either Euler angles (in degrees) or Quaternions. Quaternions are often preferred for avoiding gimbal lock and enabling smooth interpolation between rotations. 2D objects only use the Z rotation axis.

 3. Scale
	 - The Scale property affects the size of the object in relation to its original dimensions. It is represented as a vector (x, y, z), allowing for non-uniform scaling across different axes. 2D objects only use (x, y)

----
#### Hierarchy and Parent-Child Relationships

A GameObject can be the parent or child of another GameObject. When an object is "childed", it mimics changes made to the parent GameObject's transform. For example, moving the parent 3.5 units on the X axis will also move the child 3.5 units on the X axis.

----
#### Usage

Transform components can be manipulated through the Unity Editor or via scripts using C#. Common operations include moving, rotating, and scaling objects in response to user input or game events. Since it is an inherited component attached to all GameObjects, the Transform component can be accessed anytime by [[Scripting in Unity|scripts]] by using the ``transform`` keyword.