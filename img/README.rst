.. raw:: html

   <h1 align="center">

.. image:: ./img/cs.jpg
 	:width: 600px
 	:alt: SG-EDR-Test
.. raw:: html

   <br class="title">
   SG-EDR-Test
   <br>

.. image:: https://img.shields.io/github/last-commit/TH3xACE/SG_AggressorScript?style=plastic
   :target: 
   :alt: Last Commit

.. raw:: html

   </h1>

#CobaltStrike #AggresorScript #EDR #MITREAttack

.. contents:: 
    :local:
    :depth: 1

=============
INTRO
=============

**INFORMATION: The project is still under development and new functionalities will be added with time and there might be some issues, please create an issue if you found any. **

This is a custom Aggressor Script for Cobalt Strike. The script was developped to make the life of red team's easier during EDR solution testing. The script is will continously be updated. 

**Important: All the functionalities were tested with NO AV/EDR installed and some of them with AV/EDR. The main objective is to identify whether the tests are detected by them.**

=============
Overview
=============

This tool was developed with the idea to assist the Red Team in evaluating the detection of EDR/AV solutions in an automated way.

=============
Installation
=============

Requirements:
*mimikatz-kit from cobalt strike (found in dependancy folder)* 
*smbclient.py*
*truncate*
*ticketer.py*
*services.py*
*psexec.py*
*wmiexec.py*


 .. code-block:: console
 
 Step 1 :  Git clone the repo 
 
 Step 2 :  Load the cna on Cobalt Strike (Cobalt Strike > Script Manager > Load )
 
=============
Tests
=============

The tests are splitted as followed: 
--------------------------
1. User Unit Test
2. Admin Unit Test
3. User All Tests
4. Admin All Tests


=============
Usage
=============

1. Start proxy sock
--------------------------
 .. code-block:: console
 
Always setup the proxy socks 
  
 .. image:: ./img/socks.png
 	:width: 250px
 	:alt: Project

All tests with marked with [p] as below, will need proxy socks to run (need to match proxychains' config). 

 .. image:: ./img/socks-test.png
 	:width: 650px
 	:alt: Project
  
2. Set sleep
--------------------------
 .. code-block:: console
 
set sleep to 0 (not mandatory but better!) 
 
 .. image:: ./img/sleep.png
 	:width: 400px
 	:alt: Project  

3. Manually upload up.zip and prep-exf.ps1 in C:\temp
-----------------------------------------------------------
 
Prepare the files to be exfiltrated:
Run the powershell script.

  
  
4. Either choose a unit test or mulitple tests (admin or user)
-----------------------------------------------------------
 
Unit/Multiple Tests:
 .. code-block:: console
 
 .. image:: ./img/AllTests.png
 	:width: 400px
 	:alt: img-broken  
	

=============
Timeline
=============
	
The tests are related to the beacon as well as timeline. When you run the timeline, you will have access to the log related to the current beacon.

 .. image:: ./img/timeline.png
 	:width: 750px
 	:alt: img-broken  
	

=============
Excel 
=============
	
The excel file contains information about each tests (whether proxy is used, a .NET binary, cobalt strike function, windows binary,...)

 .. image:: ./img/info.png
 	:width: 1250px
 	:alt: img-broken  
	
As well as the previous tests EDR solutions.

 .. image:: ./img/tests.png
 	:width: 1250px
 	:alt: img-broken  

	

