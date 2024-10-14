#article

Writing a script in [[Unity Game Engine|Unity]] allows developers to create custom [[Component|components]], complete with their own [[Variables|variables]] and [[Functions (C-Sharp)|functions]], that can interact freely with other components. A new script can be created by right clicking an empty space in the Project window, hitting "Create" and pressing "Create [[C-Sharp|C#]] Script". After naming the script, the file will be created and the project code will re-compile. An empty script will look something like this:

```c#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class MyScript : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}

```

By default, all Unity components derive from the MonoBehaviour class, which offers life-cycle functions for [[GameObject|GameObjects]] such as `Awake()`, `Start()` and `Update()`. Default scripts also have some libraries already imported, including some system libraries needed for some basic functions and the UnityEngine library.

---
#### Heading

---
#### Related Articles
