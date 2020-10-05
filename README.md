# 2DTDMScheduler
A new tool for testing multi-vdd SoCs.
Install SQL Server Express 2019 SQLLocalDB (>v13).
SQLLocalDB is required to connect to App.
Then, run 2DTDMScheduler.exe. In the Login screen enter as username "test@tdm.sch" and as pwd "testtdm". 
Go to Configuration Tab, change credentials and select as Scheduler the 2DTDMConsole.exe file.
2DTDMScheduler can be combined with HOTSPOT thermal tool. Install HOTSPOT using WSL in windows and add the folder to PATH environment varaible.
Hotspot config file can be in a directory of you choice. Go to Configuration Tab and select as hotspot path config's folder.
Alternatively, add older hotspot.exe and hotfloorplan.exe along with the hotspot config file and select the folder as hotspot path in the configuration path.    
More info soon available.

This program is distributed as proof-of-concept for SoC TDM Test Scheduling, in the hope that it will be useful,
but WITHOUT ANY WARRANTY;
