# TDMS Test Scheduler - 2DTDMScheduler 
A new toolkit for testing DVFS-based SoCs with multiple voltage islands.
Requirements: Windows 10 OS (Toolkit can be compiled for other OS too), SQL Server Express 2019 SQLLocalDB (>v13).
Optional: Windows Subsystem for Linux (WSL) and a Linux variant for WSL.
Download application files and install SQL Server Express 2019 SQLLocalDB (>v13). SQLLocalDB is required to connect to toolkit using credentials.
Then, double-click 2DTDMScheduler.exe file. In the Login screen, enter as username "test@tdm.sch" and as pwd "testtdm". 
Go to Configuration Tab, change your credentials accordingly (it is not required for demonstration purposes) and select as Scheduler, in "Scheduler Path" option, the 2DTDMConsole.exe file (it is required the full path along with the file's name).
TDMS Test Scheduler (2DTDMScheduler) can be combined with HOTSPOT thermal tool. Install HOTSPOT in Linux variant for WSL and add the installation folder to PATH environment variable.
Hotspot config file can be in a directory / folder of you choice. Go to Configuration Tab and select this folder (hotspot config's folder - it is not required file's name) as "Hotspot Config Path".
Alternatively, add older hotspot.exe and hotfloorplan.exe files along with the hotspot config file and select their folder as "Hotspot Config Path".
In the Application files, the "exampleSOC.init2d" file can be used to demonstrate the toolkit. It includes the description of an artificial DVFS-based SoC, that consists of benchmark cores, and a TDM-based test process. Note, that the required data for each core are incorporated in the toolkit (see "aes_core.cdf" file). Thus, users can use these cores to create their artificial SoCs too (the TDM-based test process should remain the same).
To create a test process for the given SoC, user should select the option "Use Benchmark Cores" from menu button "C" (Create). Then, a window appears where user should give a name to SoC's test process (SoC configuration file). Afterwards, a message is appeared that asks from user to select an initialization file. User should press OK and select the "exampleSOC.init2d" file. The required files for the test process are produced in a new folder that has the name selected by user in the previous step. If Hotspot is available, user can also create a floorplan for the artificial SoC that can be used for thermal-oriented purposes. In this case, the floorplan switch in the configuration tab should be activated prior to any step.
To create a test schedule, user should select initially the option "Load DUT" from menu button "R" (RUN). Then, user should select the ".soc" file in the newly created folder. The toolkit will verify the selected file and it will prompt user to go to Configuration Tab. Now, user can activate new options or change parameters related to the test process (e.g Power constraints). Then, user should select the option "Load TAM" from menu button "R" (RUN) and load the ".tam" file. The toolkit will verify the selected file and it will prompt user to go again to the Configuration Tab for final checking. Finally, user should select the option "Derive Schedule" from menu button "R" (RUN) to produce a test schedule. A ".r2d" file is created in test process's folder and user can visualize it using the option "Test Schedule Graph" from menu button "S" (Schedule).

More info soon available.

This program is distributed as proof-of-concept for SoC TDM Test Scheduling, in the hope that it will be useful,
but WITHOUT ANY WARRANTY;

Find also in: https://gitlab.com/tdms-fork-group/2DTDMScheduler
