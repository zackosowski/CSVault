#article 

*For additional information, see the [Unity Manual](https://docs.unity3d.com/ScriptReference/Rigidbody2D.html) page on this topic.*

A Rigidbody2D [[component]] in [[Unity Game Engine|Unity]] is essential for adding physics behavior to 2D [[GameObject|GameObjects]]. It enables objects to react to forces and collisions in a realistic manner, making it a fundamental component for many 2D games. By adding Rigidbody2D to a GameObject, you can control its physical properties, such as mass, gravity, and drag, and determine how it interacts with other objects in the game world.

![[Rigidbody2Ddefault.png]]

---
#### Rigidbody2D Variables

| Name           | Data Type | Is Serialized? | Usage                                       |
| -------------- | --------- | -------------- | ------------------------------------------- |
| `mass`         | float     | Yes            | Determines the mass of the object.          |
| `gravityScale` | float     | Yes            | Scales the effect of gravity on the object. |
| `drag`         | float     | Yes            | Controls linear drag of the object.         |
| `angularDrag`  | float     | Yes            | Controls angular drag of the object.        |

---
#### Rigidbody2D Functions

| Name             | Return Type | Parameters       | Usage                                         |
| ---------------- | ----------- | ---------------- | --------------------------------------------- |
| `AddForce()`     | void        | Vector2 force    | Applies a force to the Rigidbody2D.           |
| `AddTorque()`    | void        | float torque     | Applies a torque to the Rigidbody2D.          |
| `MovePosition()` | void        | Vector2 position | Moves the Rigidbody2D to a specific position. |
| `MoveRotation()` | void        | float angle      | Rotates the Rigidbody2D to a specific angle.  |

---
#### Common Issues and Fixes

1. **Object Not Moving:** 
   - Ensure the Rigidbody2D is not set to "Is Kinematic."
   - Check if the mass is too high for the applied forces.
   - Verify that gravity scale is set correctly and not to 0 if you want gravity to affect the object.

2. **Unwanted Rotation:**
   - Use the "Constraints" property to freeze rotation if needed.
   - Adjust the angular drag to control the rotational deceleration.

3. **Unexpected Collisions:**
   - Make sure colliders are correctly placed and configured.
   - Check the collision layers to ensure objects are interacting as expected.

4. **Object Falling Through the Ground:**
   - Ensure colliders are correctly placed on both the object and the ground.
   - Increase the collision detection mode to "Continuous" for fast-moving objects.

---
#### Simple Example

Here is a simple example demonstrating how to apply a force to a Rigidbody2D component:

```csharp
using UnityEngine;

public class ApplyForce : MonoBehaviour
{
    public Rigidbody2D rb;

    void Start()
    {
        rb = GetComponent<Rigidbody2D>();
        rb.AddForce(new Vector2(10, 0), ForceMode2D.Impulse);
    }
}
```

In this example, a force is applied to the Rigidbody2D in the right direction when the game starts. This force is applied as an impulse, causing an immediate change in velocity.

____
#### Related Articles
[[Transform]]