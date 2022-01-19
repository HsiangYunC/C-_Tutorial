# C# Tutorial
practice with Tim Corey.

## Getting Started with C#  
### 1. [An Introduction To The C# Learning Cycle](https://youtu.be/h7aIzCkmbl8?list=PLLWMQd6PeGY2GVsQZ-u3DPXqwwKW8MkiP)
<details>  
  <summary>(notes)</summary>
  
#### - 4 steps cycle  
  1. Watch Toturial or read about something.  
  2. Build 2-5 practice projects. (not real applications. just something to understand how that piece works.)  
  3. See how each piece fits into a large whole. (real application. not only a theory)  
  4. Take what you learned in the toturial into a real application.  
</details>  

-----
### 2. [How to Install Visual Studio 2019]
<details><skip></details>

-----
### 3. [Intro to Visual Studio 2019 - What's New, What's Better, and Why You Shoule Upgrade]
<details><skip></details>

-----
### 4. [Top 10 Hidden Gems in Visual Studio - Speed Up Development Without Increasing Your Costs](https://youtu.be/xWcQhF-1hxA?list=PLLWMQd6PeGY2GVsQZ-u3DPXqwwKW8MkiP)
<details>  
  <summary>(notes)</summary>
  
  #### - 10 Tips   
  1. Quickly get to your file on disk. 
     - Right click on a tab - Open Containing Folder to open File Explorer at the file's location.  
     - Right click on a tab - Copy Full Path to copy the full path of the file.  
  2. Create auto properties when extracting an interface with Quick Actions.  
     - Tools -> Options -> Text Editor -> C# -> Advanced -> When generating properties :  
       :heavy_check_mark: prefer auto properties.  
  3. Suggest uses for types in reference assemblies and NuGet packages with Quick Actions.  
     - Tools -> Options -> Text Editor -> C# -> Advanced -> Using Directives :  
       :heavy_check_mark: Suggest using for types in reference assemblies.  
       :heavy_check_mark: Suggest using for types in NuGet packages.  
     - Access implementation using Go To Implementation.   
       - F12 : go to interface.  
       - Ctrl + F12 : go to implementation.  
  4. Do a focused search to find types, lines and other useful things using Go To.
     - Ctrl + T : helper. (like a search, but it's different kind of search. You can find things very quickly.)  
  5. Built-in refactoring using Quick Actions. (Ctrl + dot)
     - Move declaration near reference.  
     - Move type to *.cs : Create class own cs file.  
     - Remove Unnecessary Usings.  
       - Fix all occurences in : Document | Project | Solution.  
     - Object initialization can be simplified.  
       - Fix all occurences in : Document | Project | Solution.  
     - Introduce constant for "_string_".  
     - Inline temporary variable.  
  6. Easily format using Format Document.  
     - Ctrl + E , D : Edit -> Advanced -> Format Document.  
  7. C# Interactive window (Built-in REPL Editor) for quick testing and scripting.  
     - View -> Other Windows-> C# Interactive.  
     - Type a little C# code, and see how they work.  
  8. Moving whole lines up and down in the text editor.  
     - Alt + Up.  
     - Alt + Down.  
  9. Useful IntelliSense shortcuts.  
     - Ctrl + Shift + space : Puts your cusor anyway inside the (), and show you parameter list and also show you if you have overloads.  
     - Ctrl + J : Change member function.  
  10. Multi-line modifications.  
     - Shift + Alt + keyTLRB.  
     - Alt + mouse move.  
</details>  
