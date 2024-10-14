#article

*For more info, see the [Unity Manual](https://docs.unity3d.com/ScriptReference/SpriteRenderer.html) article on this component.*

The Sprite Renderer [[Component|component]] in [[Unity Game Engine|Unity]] is a rendering component that attaches a [[Sprite|sprite]] to a GameObject, allowing it to be seen in the 2D game view.

----
#### Usage

Sprite Renderers are used to display characters, enemies, objects in the game-world, etc. Common operations include changing the sprite (either in [[Scripting in Unity|script]] or via [[Unity Animation System|animators]]), changing the color of the sprite or swapping rendering layers.

----
#### Useful Properties

| **Name**         | **Property Type** | **Is Serialized?** | **Usage**                                                                                                                                                                                        |
| ---------------- | ----------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Sprite           | Sprite            | Yes                | Changes what sprite is currently being displayed by the renderer. Can be changed via script or animator.                                                                                         |
| Color            | Color             | Yes                | Changes the color of the sprite via a filter on the renderer.                                                                                                                                    |
| Sorting Order    | Int               | Yes                | Changes the rendering order of the sprite in-layer. Lower number will render the sprite below other sprites in the layer, higher number will render the sprite above other sprites in the layer. |
| Sorting Layer ID | Int               | Yes                | Changes the rendering order of the sprite out-of-layer. See [[Sprite Renderer#Sorting Layers\|Sorting Layers]] for more info.                                                                    |


----
#### Sorting Layers

Unity sorts sprite rendering layers in a priority order set by the developer through a render queue. As an example, you can have different sorting layers dedicated to the player and enemies, collectibles, environment, visual effects and more. Higher number layers will be rendered over top layers with lower numbers.

----
#### Related Articles

