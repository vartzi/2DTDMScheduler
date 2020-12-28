# 2DTDMScheduler
A new tool for testing multi-vdd SoCs.
Install SQL Server Express 2019 SQLLocalDB (>v13).
SQLLocalDB is required to connect to App.
Then, run 2DTDMScheduler.exe. In the Login screen, enter as username "test@tdm.sch" and as pwd "testtdm". 
Go to Configuration Tab, change your credentials accordingly and select as Scheduler the 2DTDMConsole.exe file.
2DTDMScheduler (TDMS Test Scheduler) can be combined with HOTSPOT thermal tool. Install HOTSPOT using Windows Subsystem for Linux (WSL) in Windows 10 and add the folder to PATH environment varaible.
Hotspot config file can be in a directory / folder of you choice. Go to Configuration Tab and select this folder (hotspot config's folder) as "Hotspot Config Path".
Alternatively, add older hotspot.exe and hotfloorplan.exe files along with the hotspot config file and select the folder as "Hotspot Config Path".
More info soon available.

This program is distributed as proof-of-concept for SoC TDM Test Scheduling, in the hope that it will be useful,
but WITHOUT ANY WARRANTY;
