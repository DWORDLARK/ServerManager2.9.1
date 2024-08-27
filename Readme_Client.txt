----------------------------------------------------------------------------------------
  Server Manager (Client) 2.9.1.x
----------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------
Version History:  
(Date Format: DD.MM.YYYY)
----------------------------------------------------------------------------------------

2.9.1:
06.05.2021

Fixed error: "Cannot focus a disabled or invisible window"
FormClose procedure added.
ServerSettings.pas
------------------------------------------------------------------
Disabled un-used Buttons and text field 
for global messages (user login main window):
Buttons:
'Reboot server now'
'Send'
Main.dfm
------------------------------------------------------------------
Maximum message interval changed from 180 to 300.
(user login main window) 
Main.dfm
----------------------------------------------------------------------------------------



----------------------------------------------------------------------------------------
2.9.1.4:

(27.08.2024)

Server settings - Maps (ServerSettings.pas)
+Maps counter for map lists
+Add Random maps
+Shuffle List (selected maps list)
+Sort List (selected maps list)
+Selection highlighter remains at last selection location
+Drag-Drop with cursor to change map order (selected maps list)
+Search (Find) map name
+Jump to next if found
+Quick remove of all selected maps


(Main)
+Local Memo (automatic save / load from local drive)
+Password Hash 

User can generate Hash after Hostname, Username, Password fields are filled.
Server service must run. It can be local. (Localhost)
After closing login error message: "Login to server failed!"
User can copy generated Hash.
Hash is generated into text field with text "Hash"
User can give Username and Hash to server ADMIN.
This helps protect user password !

Hash is generated from User name and Password !
Old password wont work if Username is changed !

----------------------------------------------------------------------------------------






