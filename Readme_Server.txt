----------------------------------------------------------------------------------------
  Server Manager (Server) 2.9.1.x
----------------------------------------------------------------------------------------

Version 2.9.1 fixes list:
06.05.2021

------------------------------------------------------------------
Client connection timeout changed from 300 to 900s
900=15 minutes

MAX_CLIENT_INACTIVITY  = 900;

HD2ServerService.pas
------------------------------------------------------------------
Disabled Console memory patching that was meant to 
accept 64 player slots.

HD2ServerService.pas
------------------------------------------------------------------
Some variables data types changed to accommodate 
preferred usable values.

HD2ServerService.pas
------------------------------------------------------------------
Disabled: application minimize to TrayIcon (Triconsi.pas)
(errors when server compiled)
Added buttons:

Start service
Stop service

TestMain.dfm
----------------------------------------------------------------------------------------




----------------------------------------------------------------------------------------
2.9.1.2
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
2.9.1.5
11.04.2025


+ Automatic save for server mpmaplist (mpmaplist_[server name])
+ Server log file is saved with date, no overwrite.







----------------------------------------------------------------------------------------

