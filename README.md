# 2DTDMScheduler
A new toolkit for testing DVFS-based SoCs with multiple voltage islands.
Requirements: Windows 10 OS (Toolkit can be compiled for other OS too), SQL Server Express 2019 SQLLocalDB (>v13).
Optional: Windows Subsystem for Linux (WSL) and a Linux variant for WSL.
Download application files and install SQL Server Express 2019 SQLLocalDB (>v13). SQLLocalDB is required to connect to toolkit.
Then, double-click 2DTDMScheduler.exe file. In the Login screen, enter as username "test@tdm.sch" and as pwd "testtdm". 
Go to Configuration Tab, change your credentials accordingly (it is not required for demonstration purposes) and select as Scheduler, in "Scheduler Path" option, the 2DTDMConsole.exe file (it is required the full path along with the file's name).
2DTDMScheduler (TDMS Test Scheduler) can be combined with HOTSPOT thermal tool. Install HOTSPOT in Linux variant for WSL and add the installation folder to PATH environment variable.
Hotspot config file can be in a directory / folder of you choice. Go to Configuration Tab and select this folder (hotspot config's folder - it is not required file's name) as "Hotspot Config Path".
Alternatively, add older hotspot.exe and hotfloorplan.exe files along with the hotspot config file and select their folder as "Hotspot Config Path".
In the Application files, the "exampleSOC.init2d" file can be used to demonstrate the toolkit. It includes the description of an artificial DVFS-based SoC, that consists of benchmark cores, and a TDM-based test process. Note, that the required data for each core are incorporated in the toolkit (see "aes_core.cdf" file). Thus, users can use these cores to create their artificial SoCs.         
More info soon available.

This program is distributed as proof-of-concept for SoC TDM Test Scheduling, in the hope that it will be useful,
but WITHOUT ANY WARRANTY;
