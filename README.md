# OpenTerminalHere-Regtweak
You can easily right click and open terminal in the exact location. 
If it doesn't work follow these steps :  
1)Open Registry Editor by pressing Windows + R, typing "regedit"--  
2)In Registry Editor, navigate to the location"HKEY_CLASSES_ROOT\Directory\Background\shell"  
3)Right-click on the "shell" key and choose "New" > "Key" to create a new key. Give it a name, such as "WindowsTerminal" for the user action or "WindowsTerminalAdmin" for the admin action.  
4)Right-click on the key you just created and choose "New" > "String Value" to create a new string value. Name it "@", and set its value to the desired display text for the context menu entry, such as "Open Terminal here" or "Open Command Prompt" etc. 
5)Right-click on the key again and choose "New" > "Key" to create a new subkey. Give it a name, such as "command". 
6)Click on the "command" key, and in the right-hand pane, double-click on the "(Default)" string value to edit its value = cmd.exe cd /d \"%V\" 

Close Registry Editor.
![1](https://user-images.githubusercontent.com/108153648/232628926-598671da-dc92-4a8e-a096-72cb8b20d95a.jpg)
![2](https://user-images.githubusercontent.com/108153648/232628931-83c8f73a-e324-4a68-a5cc-442ab96c3c5e.png)
