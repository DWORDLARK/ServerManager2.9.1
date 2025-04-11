----------------------------------------------------------------------------------------
  Server Manager 2.9.1.x
----------------------------------------------------------------------------------------

Note for server settings:
  
  Use long time interval for WatchDog.
  60sec or more.
  This can prevent ServerManager crash when some server consoles need re-start.
  
  With too short interval Server manager will try to start server console that 
  is already in process of starting and this mostly ends with ServerManager crash.
  
----------------------------------------------------------------------------------------
Version History:  
(Date Format: DD.MM.YYYY)

----------------------------------------------------------------------------------------

2.9.1:
06.05.2021

Fixed error: "Cannot focus a disabled or invisible window"
FormClose procedure added.
ServerSettings.pas

----------------------------------------------------------------------------------------
Disabled un-used Buttons and text field 
for global messages (user login main window):
Buttons:
'Reboot server now'
'Send'
Main.dfm

----------------------------------------------------------------------------------------
Maximum message interval changed from 180 to 300.
(user login main window) 
Main.dfm

----------------------------------------------------------------------------------------



----------------------------------------------------------------------------------------
2.9.1.4:
(Client program)
(27.08.2024)

Server settings - Maps (ServerSettings.pas)

*Maps counter for map lists. 
*Add Random maps. 
*Shuffle List (selected maps list). 
*Sort List (selected maps list). 
*Selection highlighter remains at last selection location.
*Drag-Drop with cursor to change map order (selected maps list).
*Search (Find) map name. 
*Jump to next if found. 
*Quick remove of all selected maps.


(Main). 
*Local Memo (automatic save / load from local drive).
*Password Hash. 

----------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------
v: 2.9.1.2
(Server)
27.08.2024

+Server reads map names from individual maplist files.

----------------------
How to use:

Server uses default mpmaplist.txt to load mission data (mission folder and items/player equipment/objectives).

Each server uses own maplist to load map list into client program to fix 255 enrty limit.

Example:
Server named: "co-op1" works with maplist file: mpmaplist_co-op1.txt  (mpmaplist_[server name])
Servers own maplist can only store names ! (no need for add items/ojectives)

If ServerManager starts, it creates copy of mpmaplist.txt with only names, discarding all other data.
File: "mpmaplist_Names_Only.txt"
Server Admin can use this file to store map names into server own maplist (mpmaplist_[server name])

! ! !  Server console is not able to load map / start service if mission entry is only present in
server own maplist file (mpmaplist_[server name])
Full copy of mission data (items/objectives) must be present in mpmaplist.txt, with same mission name.

----------------------------------------------------------------------------------------

v: 2.9.1.5
(Server)
11.04.2025

----------------------
+ServerLog file is not deleted after ServerManager restart.
  (Date is added to Logfile name)

+ mpmaplist with server name  (mpmaplist_[server name]) is created when
    user creates new server.
    No need for user to creat in manually !

----------------------------------------------------------------------------------------
