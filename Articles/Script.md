In programming, a script is a type of program that is typically written in a scripting language and is designed to automate tasks or execute a sequence of instructions. Scripts are often interpreted rather than compiled, meaning they can be run directly by an interpreter without the need for a separate compilation step.

Key characteristics of scripts include:

1. **Ease of Use**: Scripts are usually simpler and shorter than full-fledged programs, making them easier to write and modify.

2. **Interpreted Languages**: Common scripting languages include Python, JavaScript, Ruby, and Bash. These languages allow for quick development and testing.

3. **Automation**: Scripts are often used to automate repetitive tasks, such as file manipulation, data processing, and system administration tasks.

4. **Integration**: Scripts can often integrate with other software or systems, allowing them to control or interact with various applications.

5. **Cross-Platform**: Many scripting languages are designed to be cross-platform, allowing scripts to run on different operating systems with little or no modification.

----

#### Scripting in Unity

Writing a script in [[Unity Game Engine|Unity]] allows developers to create custom [[Component|components]], complete with their own [[Variables|variables]] and [[Functions (C-Sharp)|functions]] and interact freely with other components. A new script can be created by right clicking an empty space in the Project window, and pressing "Create [[C-Sharp|C#]] Script". After naming the script, the file will be created and the project code will re-compile. An empty script will look something like this:

```c#
//put code here
```

By default, all Unity components derive from the MonoBehaviour class, which offers life-cycle functions for [[GameObject|GameObjects]] such as `Awake()`, `Start()` and `Update()`