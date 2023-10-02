<h1>Windows Artifacts Project</h1>


<h2>Description</h2>
The project is centered on digital forensics, specifically extracting and interpreting critical information from system artifacts. Using specialized tools, the endeavor dives deep into LNK files, Jump Lists, and various registry hives like NTUSER.DAT, SYSTEM, and UsrClass.Dat. The analysis uncovers valuable insights about user activities, software installations, and system configurations, revealing a comprehensive understanding of user behaviors and the system's inner workings. It includes the following tasks:
<br />
<br />
- <b>Parsing LNK files using LECmd and analyzing / extracting useful information</b> 
<br />
- <b>Paring Jump Lists using JLECmd and analyzing / extracting useful information </b>
<br />
- <b>Analyzing the NTUSER.DAT Registry Hive using RegRipper or Registry Explorer and extracting useful information</b>
<br />
- <b>Analyzing the SYSTEM Registry Hive using RegRipper or Registry Explorer and extracting useful information</b>
<br />
- <b>Analyzing the UsrClass.Dat Registry Hive using RegRipper or Registry Explorer and extracting useful information</b>
<br />


<h2>Software and Utilities Used</h2>
- <b> LECmd </b>
<br />
- <b>JLECmd</b>
<br />
- <b>Registry Explorer</b>
<br />
- <b>MFT Stampede</b>
<br />
- <b>RegRipper</b>
<br />
- <b>ShellBags Explorer</b>

<h2>Environments Used </h2>
- <b>Windows 10 Pro</b>


<h2>Lab Walkthrough</h2>
<h3>Parse and Analyze LNK Files</h3>
<p align="center">

Parse the LNK files located in the “Recent” folder using LECmd<br/>
<img src="https://i.imgur.com/s2K1kW5.png" height="80%" width="80%" alt="Log into Windows"/>
<br />
<br />
Answer the following questions: 
<br />
<br />
1) What was the file size in bytes of “Great Horned Owl.jpg” the last time it was opened?
<img src="https://i.imgur.com/hk10Q0p.png" height="80%" width="80%" alt="Log into Windows"/>
<br />
<br />
64476 bytes
<br />
<br />
3) What is the VSN associated with the volume from which a folder called “rust” was
opened?
<img src="https://i.imgur.com/GlJo4n8.png" height="80%" width="80%" alt="Log into Windows"/>
<br />
<br />
Volume Serial Number
6C191B65
<br />
<br />
5) How many different computer names are present in the collection of LNK files?
<img src="https://i.imgur.com/2cDortR.png" height="80%" width="80%" alt="Log into Windows"/>
<br />
<br />
4
<br />
<br />
8) Based on analysis of the LNK files, what time did the Max Powers user account start
downloading a KeePass .zip archive?
<img src="https://i.imgur.com/XcldsrL.png" height="80%" width="80%" alt="Log into Windows"/>
<br />
<br />
2018-04-26 16:29:30
<br />
<br />
10) How many different cloud storage services are referenced by the LNK files?
<img src="https://i.imgur.com/xH1sopa.png" height="80%" width="30%" alt="Log into Windows"/>
<img src="https://i.imgur.com/N6XmWvv.png" height="80%" width="30%" alt="Log into Windows"/>
<img src="https://i.imgur.com/Yl8Dju1.png" height="80%" width="30%" alt="Log into Windows"/>
<br />
<br />
3 different cloud storage services
<br />
<br />
12) What is the name of the computer on which the “rich.pdf” file is stored?
<img src="https://i.imgur.com/4Fl9OLQ.png" height="80%" width="30%" alt="Log into Windows"/>
<br />
<br />
Inconclusive
<br />
<br />
14) Based on analysis of the LNK files, what type of animals is the user of the “Sarah M”
account interested in?
<img src="https://i.imgur.com/eGwmEqq.png" height="80%" width="30%" alt="Log into Windows"/>
<br />
<br />
Mostly owls
<br />
<br />
16) What is the MFT record number (in decimal) of the file opened from a removable device
on 02/02/2017 22:38:36 UTC?
<img src="https://i.imgur.com/wgwqhGY.png" height="80%" width="30%" alt="Log into Windows"/>
<br />
<br />
3769120
<br />
<br />
18) When was the file “Owl_Emergency_Care.pdf” last modified in the “New Pet Care”
directory?
<img src="https://i.imgur.com/1X8Q39X.png" height="80%" width="30%" alt="Log into Windows"/>
<br />
<br />
Target Modified
2017-01-31 19:09:01
<br />
<br />

<h3>Parse and Analyze Jump Lists</h3>
<p align="center">

Parse the Jump Lists located in the “Recent\AutomaticDestinations” folder using JLEmd and
answer the following questions:
<img src="https://i.imgur.com/8XI3X1M.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Answer the following questions:
<br />
<br />
1) What is the name of the largest file referenced by the jump list records?
<img src="https://i.imgur.com/gnzPPCN.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Snowy Owl.jpg
<br />
<br />
3) What is the name of the subdirectory within the “maxpowers” user account folder where
a Python script appears to be stored?
<img src="https://i.imgur.com/xDrUTPc.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
"Stuff"
<br />
<br />
4) When was the file “C:\Users\Win7\Documents\Personal.docx” last opened?
<img src="https://i.imgur.com/tsJsuK0.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Last Modified
2014-03-02 18:50:39
<br />
<br />
5) When was the file “Pygmy Owl.jpg” created in the “Pets” directory?
<img src="https://i.imgur.com/u3gm9wv.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Target Created
2017-01-27 17:19:14
<br />
<br />
7) What is the computer name of the system from which “EventIpAddresses.xlsx” was
opened?
<img src="https://i.imgur.com/vH5s8Qd.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Machine ID
desktop-edslqm8
<br />
<br />
8) How many different computer names are present in the collection of jump list records?
<img src="https://i.imgur.com/2dVXz9W.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
3
<br />
<br />
10) Based on AppID, how many different versions of Excel are represented in the collection of
jump list records?
<img src="https://i.imgur.com/Frjnbmz.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
2 versions
<br />
<br />
11) Based on the jump list records available for analysis, what is the most recently used web
browser?
<img src="https://i.imgur.com/UF3n9wD.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Based on its AppID and last modified timestamp, Microsoft Edge
<br />
<br />

<h3>Analyzing the NTUSER.DAT Registry Hive</h3>
<p align="center">

Parse the NTUSER.DAT registry hive located in the “Reg” folder using RegRipper and/or view the
hive contents using Registry Explorer
<img src="https://i.imgur.com/fjDCiZF.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Answer the following questions:
<br />
<br />
18) What version of Python was downloaded to this system?
<img src="https://i.imgur.com/fjDCiZF.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Version 2.7
<br />
<br />
20) What is the name of the directory in which “Starter.docx” is stored?
<img src="https://i.imgur.com/Z4k60iC.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
C:\Users\maxpowers\Documents\Starter.docx
<br />
<br />
22) What version of KeePass appears to be installed or used on this system?
<img src="https://i.imgur.com/4pWHPM9.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Version 1.35
<br />
<br />
24) When was the file “Database.kdb” last opened?
<img src="https://i.imgur.com/XD0HlSk.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Opened On
2018-04-26 16:32:46
<br />
<br />
26) What is the file extension most recently opened by this user account?
<img src="https://i.imgur.com/AKXZq30.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
.lnk
<br />
<br />
28) Based on the UserAssist subkey, how many times was “mspaint.exe” executed by this
user account?
<img src="https://i.imgur.com/W4cv6Qn.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
7 times
<br />
<br />
30) Based on the “Run” subkey, how many programs are configured to start when this user
account logs on to the system?
<img src="https://i.imgur.com/W4PXpEF.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
1 - OneDrive
<br />
<br />
32) When was the program “atom” installed on the system?
33) <img src="https://i.imgur.com/9UR4MG0.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
April 9, 2018
<br />
<br />

<h3>Analyzing the SOFTWARE Registry Hive</h3>
<p align="center">

Parse the SOFTWARE registry hive located in the “Reg” folder using RegRipper and/or view the
hive contents using Registry Explorer
<img src="https://i.imgur.com/fjDCiZF.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Answer the following questions:
<br />
<br />
Based on the “Run” subkey, how many programs are configured to start when this
computer starts?
<img src="https://i.imgur.com/gQ7luKY.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
4 Programs
<br />
<br />
27) What is the Security Identifier (SID) associated with the “Sarah M” user account?
<img src="https://i.imgur.com/ef0Xhlw.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
S-1-5-21-929903582-3707417421-3176878646-1002
<br />
<br />
28) What is the Volume Serial Number (VSN), in decimal, associated with the SanDisk Cruzer
Glide USB device that was connected to the system?
<img src="https://i.imgur.com/3zahrJ3.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
2159839650
<br />
<br />
29) What is the LastWrite time associated with the
“Microsoft\DirectPlayNATHelp\DPNHPAST” subkey?
<img src="https://i.imgur.com/pTTTRV4.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
2017-01-27 02:32:37
<br />
<br />
30) What is the name of the “Foxit Software” application that is installed on the system?
<img src="https://i.imgur.com/PtHVBUG.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Foxit Phantom
<br />
<br />
31) What version of operating system is installed?
<img src="https://i.imgur.com/ABoqWSG.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Windows 10 Pro Version 6.3
<br />
<br />
32) When was the operating system installed?
<img src="https://i.imgur.com/jq9gYEl.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
2017-01-27 02:58:47
<br />
<br />

<h3>Analyzing the SYSTEM Registry Hive</h3>
<p align="center">

Parse the SYSTEM registry hive located in the “Reg” folder using RegRipper and/or view the hive
contents using Registry Explorer
<img src="https://i.imgur.com/q3zjOGV.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Answer the following questions:
<br />
<br />
33) Based on the USBSTOR subkey, how many USB devices appear to have been connected
to this system?
<img src="https://i.imgur.com/xUYGQif.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
2 Devices
<br />
<br />
34) What is the serial number of the SanDisk Cruzer Glide device?
<img src="https://i.imgur.com/CaJ8j5l.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
20051739911AEEC1DE29&0
<br />
<br />
35) What is the computer name of this system?
<img src="https://i.imgur.com/l0nC9n1.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
DESKTOP-KLOQJ0V
<br />
<br />
36) When does the computer name of this system appear to have been last changed or set?
<img src="https://i.imgur.com/yYN8p4D.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
2017-01-27 02:32:40
<br />
<br />
37) Based on the ShimCache, what is the last modification time of
“C:\WINDOWS\sysWOW64\wbem\wmiprvse.exe”?
*Note: Registry Explorer would crash when trying to open the AppCompatCache key so I had to use RegRipper
<img src="https://i.imgur.com/P51EMrf.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
2016-07-16 11:42:56
<br />
<br />
38) For the “Standard Profile” configuration of the Windows firewall, what is the default
logging location for firewall logs?
<img src="https://i.imgur.com/Fuz8QOU.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
%systemroot%\system32\LogFiles\Firewall\pfirewall.log
<br />
<br />

<h3>Analyzing the UsrClass.Dat Registry Hive</h3>
<p align="center">

Parse the UsrClass.Dat registry hive located in the “Reg” folder using Shellbags Explorer
<img src="https://i.imgur.com/M2fA5IV.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Answer the following questions:
<br />
<br />
What is the name of the .zip file located in the user’s Downloads directory?
<img src="https://i.imgur.com/fHnhsa5.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
webbrowserpassview.zip
<br />
<br />
40) Based on the user’s interaction with the Control Panel applet, what type of activity does
it appear the user was conducting in the Control Panel?
<img src="https://i.imgur.com/vYVSd4F.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
Change an Account within User Accounts: This indicates that the user was likely reviewing or potentially making modifications to an account on the system. 
<br />
System within System and Security: This indicates the user was accessing system properties, which is where details about the computer (e.g., computer name, system type, RAM, etc.) are displayed. Additionally, this is where one might go to join a domain, view computer performance information, or view/change the computer's name.
<br />
<br />
41) What is the first interacted timestamp of the “C:\Python27\Lib\site-packages\requests2.18.4.dist-info” directory?
<img src="https://i.imgur.com/dn3M1lg.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
2018-03-13 18:50:10.975
<br />
<br />
42) Based on shellbags analysis, how many subdirectories are visible within the “C:\Projects”
directory?
<img src="https://i.imgur.com/JajCzeH.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
5 Subdirectories
<br />
<br />
43) Based on shellbags analysis, what is the name of the last directory with which this user
account interacted?
<img src="https://i.imgur.com/pfq8sUg.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />
C:\Users\maxpowers\Documents 2018-05-04 22:00:48.984
<br />
<br />
<h2>Conclusion </h2>
This digital forensic exploration successfully delved into various system artifacts, revealing intricate details of user activities and system configurations. By employing specialized tools, the project was able to extract crucial data from LNK files, Jump Lists, and diverse registry hives. This in-depth analysis not only showcases the vast capabilities of modern forensic methodologies but also underscores the importance of such investigations in understanding user behaviors and ensuring cybersecurity.
