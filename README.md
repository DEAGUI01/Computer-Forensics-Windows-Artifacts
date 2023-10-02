<h1>Windows Artifacts Project</h1>


<h2>Description</h2>
This project involves a comprehensive exercise in forensic image conversion and analysis using tools like FTK Imager and WinHex. I delve deep into the technicalities of forensic imaging and analysis which is a critical skill in the field of digital forensics. This hands-on project is structured into several sections which that go through various tasks including forensic image conversion, working with alternate data streams (ADS), and parsing Master File Table (MFT) records. It includes the following tasks:
<br />
<br />
- <b>Forensic Image Conversion using FTK Imager</b> 
<br />
- <b>Working with Alternate Data Streams</b>
<br />
- <b>Parsing MFT Records</b>
<br />


<h2>Software and Utilities Used</h2>
- <b> LECmd </b>
<br />
- <b>JLECmd</b>
<br />
- <b>Registry Explorer</b>
<br />
- <b>MFT Stampede</b>

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

Parse the NTUSER.DAT registry hive located in the “Reg” folder using RegRipper and/or view the
hive contents using Registry Explorer
<img src="https://i.imgur.com/fjDCiZF.png" height="80%" width="80%" alt="Investigate FAT32"/>
<br />
<br />


<h2>Conclusion </h2>
This project embarked on a meticulous journey through the intricacies of forensic image conversion and analysis, establishing a potent framework for delving deep into the realms of digital forensics. Here are the significant takeaways and conclusions drawn from this endeavor:

<b>Comprehensive Skill Development:</b> The project facilitated a deep understanding and skill development in forensic image analysis, an essential skill in the contemporary digital forensics domain. This was significantly aided by hands-on experience with tools like FTK Imager and WinHex.

<b>Hands-On Experience with ADS:</b> Working with Alternate Data Streams (ADS) proved to be an enlightening experience, offering insights into the hidden layers of file systems and how they can be utilized for forensic analysis.

<b>Deep Dive into MFT Records:</b> Parsing Master File Table (MFT) records was a challenging yet rewarding task, unveiling the deep-seated data structures and timestamps that are essential in forensic investigations. The MFT Stampede was particularly useful in this regard.

<b>Practical Application of Concepts:</b> The project not only imparted theoretical knowledge but also emphasized practical applications, providing a real-time simulation of forensic analysis processes. This will undoubtedly prove invaluable in real-world forensic analyses.

<b>Understanding File System Properties:</b> The project threw light on the nuanced differences between various file systems like NTFS and FAT32, particularly concerning features like ADS, helping in grasping the broader picture in digital forensic analysis.

<b>Enhanced Proficiency with Forensic Tools:</b> Through the series of tasks undertaken during this project, there was a noticeable enhancement in proficiency with using digital forensic tools and utilities, setting a strong foundation for future endeavors in the field.

<b>Preparation for Advanced Analysis:</b> This project served as an excellent precursor to more advanced analyses in the realm of digital forensics, paving the way for deeper exploration and research in this rapidly evolving field.

<b>Visual Engagement:</b> The addition of visual aids in the walkthrough provided a visual, immersive learning experience, allowing for a more straightforward and practical approach to understanding the concepts at hand.
