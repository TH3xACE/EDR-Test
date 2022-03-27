.. raw:: html

   <h1 align="center">

   <br class="title">
   EDR-Test
   <br>

.. raw:: html

   </h1>

#CobaltStrike #AggresorScript #EDR #MITREAttack

.. contents:: 
    :local:
    :depth: 1

=============
INTRO
=============

**Who said Cobalt Strike was meant to be use only as an offensive tool (Red Team)?**

As part of the purple team activity, I was involved in testing different EDRs solutions to evalutate their detection capabilities by emulating attacks using Techniques, Tactics, and Procedures (TTP) used by adversaries. I wanted to automate the tests, to make it easier for us as well as to make a consistent and effective comparison between the different solutions.

My first consideration was the project **Atomic Red Team** , it is a really nice project and initiative but despite that, some of my objectives would not be achievable such as not to use powershell, having better flexibility and some custom (ninja) feature.  


Link: https://github.com/redcanaryco/atomic-red-team

After some online search (thanks to Dr. google) to find some other (FREE) alternatives. I came to the conclusion that if I wanted to meet all my objectives, I needed to get the hand dirty. So I decided to go for my own project but what Programming Language to use ? Since at that time, I was aiming to to improve my coding skills in Cobalt strike Aggressor Script (.cna) and that on top of that, it would allow me to achieve all my objectives, it was the way to go.








 .. image:: ./img/tool-header.png
 	:width: 1000px
 	:alt: Project
=============

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

	

