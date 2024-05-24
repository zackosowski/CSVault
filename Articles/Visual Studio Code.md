#article

Visual Studio Code, often abbreviated as VS Code, is a popular [[IDE (Integrated Development Environment)]] developed by Microsoft. It is widely used by programmers for writing and editing code in various [[Programming Language|programming languages]].

---
#### Key Features

**Cross-Platform:** 
	VS Code runs on Windows, macOS, and Linux, making it accessible to users on different [[Operating System|operating systems]].

**Extensibility:**
	One of VS Code's strongest features is its extensibility. Users can install extensions to add new languages, [[Debugging|debuggers]], themes, and other tools, customizing the editor to fit their specific needs.

**IntelliSense:**
	This feature provides smart code completions based on [[Variables|variable]] types, [[Functions|function]] definitions, and imported modules, helping programmers write code more efficiently.

**Integrated Git:**
	VS Code includes built-in [[Git and GitHub|Git]] support, allowing users to manage version control without leaving the editor.

**Debugging:**
	The editor offers powerful debugging tools, enabling users to set [[breakpoints]], inspect variables, and control execution flow directly within the code.

---
#### User Interface

###### A) Activity Bar
- Located on the far left.
- Provides quick access to different views.
	- **Explorer**: Shows the project [[Computer File Systems|files and directories]].
    - **Search**: Allows searching across files in the workspace.
    - **Source Control**: Provides integration with version control systems like [[Git and GitHub|Git]].
    - **Debugger**: Built-in [[debugging]] tool
    - **Extensions**: Lets you browse, install, and manage extensions.
###### B) Primary Side Bar
- Displays the contents of the selected activity from the Activity Bar.
 - The most common view is the explorer as shown in the image below.
###### C) Editor Groups
- The central area where you edit your files.
- Supports multiple editors and split views, allowing side-by-side file editing.
- Each editor tab can be split horizontally or vertically.
###### D) Panel
- Located at the bottom by default but can be moved to the side.
- Houses views such as:
    - **Output**: Displays output from various processes, like build tools or servers.
    - **Terminal**: Integrated [[Terminal|terminal]] for running command-line tasks.
    - **Problems**: Lists [[errors]] and [[Warning|warnings]] in the project files.
    - **Debug Console**: Displays output and allows input during debugging.
###### E) Status Bar
- Located at the bottom of the window.
- Provides information about the open file and the project such as [[Character Mapping|encoding]], line ending, file type, and cursor position.
- Shows background tasks and errors or warnings.

![[vscode1.png]]

---
#### Getting Started

Open VS Code by searching for it on your computer
* Before opening, right click -> pin to taskbar
* Install Extensions:
	* `ms-python.python`
	* `beardedbear.beardedtheme -> Black & *` (Class theme, optional)
	* `usernamehw.errorlens`
	* `pkief.material-icon-theme`
* Change Settings
	* Text Editor -> Cursor ->
		* Cursor Blinking -> Expand
		* Enable "Cursor Smooth Caret Animation"
	* Right-click Activity Bar -> Move Primary Side Bar Right
	* Top of screen -> Terminal -> New Terminal
		* Drag terminal below editor
	* Right-click status bar -> Hide Status Bar

---
#### Setting up GitHub for VS Code

1. Open Visual Studio Code
2. Top of VS Code -> View -> Terminal
3. Type	```git config --global user.email "YOUREMAIL@mystma.org"```
4. Press enter
5. Type	```git config --global user.name "your github username"```
6. Press enter