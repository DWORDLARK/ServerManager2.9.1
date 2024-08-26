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
