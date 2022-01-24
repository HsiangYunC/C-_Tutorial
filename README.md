# C# Tutorial
practice with Tim Corey.

## Getting Started with C#  
### 1. [An Introduction To The C# Learning Cycle](https://youtu.be/h7aIzCkmbl8?list=PLLWMQd6PeGY2GVsQZ-u3DPXqwwKW8MkiP)
<details>  
  <summary>(more)</summary>
  
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
  <summary>(more)</summary>
  
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
  
-----
### 5. [15 Visual Studio Editor Tips including Intellicode and EditorConfig](https://youtu.be/qv6ZflueASY?list=PLLWMQd6PeGY2GVsQZ-u3DPXqwwKW8MkiP)  
<details>
  <summary>(more)</summary>
  
  #### - 15 Tips 
  1. IntelliCode  
    - Extensions -> Manager Extensions -> Installed -> Visual Studio IntelliCode  
  2. Personalized Intellicode
    - Tools -> Options -> IntelliCode -> (setting IntelliCode)
    - View -> Other Windows -> IntelliCode Model Management
  3. Code Styles
    - Tools -> Options -> Text Editor -> C# -> Code Style
      - Naming
      - Formatting  
  4. Editor Config  
    - Tools -> Options -> Text Editor -> C# -> Code Style -> General -> Generate .editorconfig file from settings  
    - Project Solution -> Add -> New EditorConfig (IntelliCode)  
    - Tools -> Options -> IntelliCode -> General -> EditorConfig inference -> Enable  
  5. Solution Performance : helps you give into visual studio faster  
    - Tools -> Options -> Projects and Solutions  
  6. Code Cleanup  
    - Ctrl + K , E : Run Code Cleanup  
  7. Project/Solution-wide Code Cleanup  
    - Solution Explorer -> (mouse right click) -> Analyze and Code Cleanup -> Run Cleanup  
  8. Paste as JSON  
    - Edit -> Paste Special -> Paste JSON As Classes  
  9. Quick Actions and Refactoring  
    - Invert if  
    - Use Pattern matching  
  10. Discard Character  
      ```cs
      (string fn, string ln) = GetNames();
      var (fn, _) = GetNames(); // don't care about lastname
      public static (string firstName, string lastName) GetNames()
      {
         return ("Tim", "Corey");
      }
      ```  
  11. XAML Hot Reload  
    - UI change and reload immediately  
    - XAML Pop-out Option (bonus)  
  12. Pin Properties in List
    - for debug easier  
  13. Clipboard Ring  
    - Ctrl + Shift + V : paste list  
    - Windows + V : Windows Clipboard Ring (bonus)  
  14. Toolbox Code Storage  
    - Storage the code you want to remember. rename  
    - drag code into toolbox  
  15. Universal Search  
    - Ctrl + Q  
      - quick way to create new file (enter : add class)  
      - quickly setting (enter : themes / intellicode)  
    - Vertical document tab (bonus)  
      - Options -> Environment -> Preview Features :  
        :heavy_check_mark: Vertical document tab layout  
      - Right click on tabs -> Set Tab Layout -> Left / Top / Right  
</details>

-----
### 6. [How to Get Help Online as a Software Developer]    
<details><skip></details>
  
-----
### 7. [C# Debugging: Breakpoints]  
<details><skip></details>
  
-----
### 8. [C# Debugging: Breakpoints]  
<details><skip></details>
    
-----
### 12. [Working With The File System in C# - Managing Folders and Files](https://youtu.be/9mUuJIKq40M?list=PLLWMQd6PeGY2GVsQZ-u3DPXqwwKW8MkiP)  
<details>
  <summary>(more)</summary>

  #### - File System Demo
  1. reading all directories in the path specified  
      ```cs
      // using System.IO;
  
      string rootPath = @"E:\Temp\Demos\FileSystem";
  
      // "*" : filter
      // SearchOption : TopDirectoryOnly / AllDirectories
      string[] dirs = Directory.GetDirectories(rootPath, "*", SearchOption.AllDirectories);  
  
      foreach (string dir in dirs)
      {
          Console.WriteLine(dir);
      }
  
      var files = Directory.GetFiles(rootPath, "*.*", SearchOption.TopDirectoryOnly);
  
      foreach (string file in files)
      {
          Console.WriteLine(file);
      } 
     ```
  2. reading all files in the path specified (directories included)  
      ```cs
      // using System.IO;
  
      string rootPath = @"E:\Temp\Demos\FileSystem";
  
      // "*.*" : filter
      // SearchOption : TopDirectoryOnly / AllDirectories
  
      var files = Directory.GetFiles(rootPath, "*.*", SearchOption.TopDirectoryOnly);
  
      foreach (string file in files)
      {
          Console.WriteLine(file);
          Console.WriteLine(Path.GetFileName(file)); // getting file path only
      } 
     ```  
  3. reading all files (directories excluded), omitted file extensions, getting file path only
  
  9:43
  
  
</details>
