YOU NEED JAVA 18 TO PLAY 1.19.2 MODPACKS. THIS CAN BE INSTALLED HERE https://adoptium.net/temurin/releases/?version=18 (install and run the 64bit .msi file)
If your server still doesn't launch with Java 18, uninstall other Java versions! This can be done by going to Programs and Features, then typing the letter "j" to search for versions of Java.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

ONLY USE THESE FILES TO RUN THE SERVER:
Windows = start.ps1
Linux = start.sh
(DO NOT USE THE .jar TO RUN THE SERVER!)
Note that the file extensions (the .sh and the .ps1) will not show if you haven't enabled them. Instead, you can look for "Windows Powershell" to the right of the file named "start"

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Below is a list of commonly asked questions. If you have a question not answered in this document, please ask the question in our Discord: https://lunapixel.studio/discord

	Q: How do I start the server?
A: Right click the Start.ps1 file and Open with Powershell. 
	Q: How do I join my server?
A: 1) Install the modpack using a modded launcher (Curseforge, GDLauncher, ATLauncher, etc)	2) go to the Multiplayer tab in the main menu	3) click Direct Connect and type localhost
	Q: How do others join my server?
A: They will connect using your Public IP Address, which can be found by typing "my ip address" into Google. If people are unable to join with this IP, find a portforwarding guide online.
	Q: How do I allocate more RAM?
A: 1) Open the variables.txt text file    2) On line 8, you can add Java arguments inbetween the quotation marks. -Xmx8g will set maximum RAM usage to 8 gigabytes.
	Q: Should I be worried about errors in the console?
A: Unless there is something that is not working as expected, don't mind any errors. 99% of them mean nothing.
	Q: Why is my server so laggy?
A: There are a few things you can do to for server lag:
 1) Follow this guide for optimal Java args. Please note that these can cause instability or worsened performance for some people: https://github.com/brucethemoose/Minecraft-Performance-Flags-Benchmarks
 2) If lag persists, do the following command ingame:
/spark profiler --interval 100
 3) Check the Spark Profiler website link that shows up in chat/console and check if your server is using all of the memory. You can allocate more memory accordingly.
 4) On the Spark Profiler website, you can also check what processes are using the most resources. Our Discord community can help you further if necessary.
	Q: How do I make my server public?
A: 1) To make your server available to the public, you have to go into the Server's Config folder > Navigate to BHMenu Folder and edit the bhmenu-public_server_list.properties file
2) Set it to True to enable your server to be viewed publicly on the Server Browser
3) To get your server registered on the Server Browser you need to post your server on https://minecraft.multiplayerservers.net/ or click the "Add Server" button on the Server Browser tab in the Multiplayer Menu.
Servers hosted using Bisect get placed higher on the server list. Make sure it's posted under the correct modpack or it will not show up in the ingame server browser. 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
IMPORTANT FOR WINDOWS 11 22H2 USERS!:
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
	Q: When I open Powershell, it closes immediately! (This can also solve other issues!)
A: This is likely an issue with Powershell itself. Here is an alternative method of opening the start.ps1:
1) Press the Windows key, type Powershell and run as Administrator
2) Run the following: set-executionpolicy remotesigned
3) Agree by typing A
4) Run the start.ps1 again by Right click the Start.ps1 file and Open with Powershell.
5) Now it should work (If it does not work, restart your PC and try running again)

Windows 11 users can also try doing Step 1-5 of the alternative method of opening the start.ps1 (which can be found above) and then running the following command: Unblock-file -Path InsertFilePathHere

After running this command, the start script should work again. If not, use the guides below.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

IF YOU DO NOT WANT TO FOLLOW THE ABOVE FIX THEN YOUR ONLY OPTION IS MANUAL INSTALLATION:

New Windows 11 22H2 Update causes the PowerShell not to work. I suggest these Videos for Manual Installation:
FORGE 1.19.2: https://www.youtube.com/watch?v=3HD0ibIpO-A
FABRIC: https://www.youtube.com/watch?v=b2W1Xb7nLKo
Make sure to Install the Server in our ServerPacks so it can use the correct files.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

LASTLY, IF YOU DO NOT WANT TO FACE THESE ISSUES WE RECOMMENED BISECT HOSTING:
Approx. $10 - $25 a month depending on what plan you choose. You can also get 25% off with Code LunaPixel.

Go to https://www.bisecthosting.com/LunaPixel and order a plan which fits you. We suggest 1GB per player but nothing lower than 4GB as the server needs at least 3GB to run.