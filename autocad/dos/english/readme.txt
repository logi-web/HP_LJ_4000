Readme File for the Hewlett-Packard HP-GL/2 and HP RTL driver for AutoCAD 
-------------------------------------------------------------------------

Product name:    HP-GL/2 Driver for AutoCAD
------------     Releases 10, 11, 12, 13, 14 (v4.0)

Version number:  v4.0
--------------
Language(s) supported: English, French, Italian, German, Spanish, Japanese,
---------------------  Simplified Chinese, Traditional Chinese, Korean.

Products supported:     
------------------      
      HP DesignJet series (except the original DesignJet)
      HP DraftMaster SX/RX/MX
      HP DraftMaster Plus series
      HP DraftPro Plus
      HP LaserJet series
      HP PaintJet XL 300
      HP 7600 series Electrostatic plotter models


System requirements:  The version of AutoCAD for which you want to install
-------------------   this driver must already be installed on your PC.
                      AutoCAD must have been executed at least once before
                      installing the driver in order to make sure it is
                      properly configured and that the file ACAD.CFG (or
                      ACADNT.CFG or ACAD14.CFG) has been created. 
                      


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Driver notes: (general for all versions)
----------------------------------------


Network Installation
--------------------
Keep in mind these requirements for installing this driver if you run
AutoCAD from a server:

1.- The driver can be installed in the server and can be used from any
    computer attached to it.

2.- You need write permission for the server’s hard drive directories.
    If you don't have such permission, your System Administrator or another
    user with proper access rights must run the installation.

3.- No AutoCAD session can be running while you install the driver.  You
    may need to ask your workmates to quit their AutoCAD sessions during
    the installation process.


File Transfer Error
-------------------
If you receive a "General file transfer error" during the installation of
this driver, make sure that you have write permissions for the directory
and all subdirectories that you have selected to install to.


If you are upgrading your existing driver to v4.0
-------------------------------------------------
If your AutoCAD configuration is already setup to use an older version of 
this driver (v3.3 or earlier) note that you will need to repeat the process
of plotter configuration in AutoCAD so that it can use the driver version
4.0.  Furthermore the installation process will remove your older version
of the driver when it installs this new version.

See below for additional notes for specific systems.


Cancelling a Job
----------------
It is not possible to cancel a job using the Status Monitor if the job is
inside a nest of jobs.  However, the cancel will be effective on the
following nest if it contains pages of the canceled job. 


Multiple AutoCAD sessions
-------------------------
Although AutoCAD releases 13 and 14 allow several sessions to run
simultaneously, the driver can only work for one of them.


Minimum media size
------------------
When you specify a User Size (in PLOT, HPMPLOT or HPRENDER) that is smaller
than A4 and you are using roll media, the drawing will be plotted the right
size but the media could be cut to A4 size.


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


AutoCAD application notes:

AutoCAD release 12 for Windows users
------------------------------------

1.- Make sure you have installed the latest version (C4 or higher) 
    of AutoCAD r12 for Windows.  Autodesk provides a free upgrade 
    for all AutoCAD for Windows users to this version.


2.- In order to be sure that your HP driver for AutoCAD is
    correctly installed, check the contents of the following files:

    File 1: ACAD.ADS

        This file, which can be found by default in the directory
        C:\ACADWIN, should include the following instructions:

        acadapp
        C:\ACADWIN\SUPPORT\HPMPLOT.EXE


    File 2: WIN.INI

        This file, which can be found by default in the directory
        C:\WINDOWS, should include under the section: 

        [hpgl2acaddrv]

        the following line:

        config=C:\ACADWIN\

        or wherever the AutoCAD configuration is placed.


3.- You can only install the HP-GL/2 driver for one 
    AutoCAD Release 12 configuration per PC.


AutoCAD release 13 for Windows users
------------------------------------

This version requires a significant amount of memory. If error
messages are encountered, we recommend you add more memory to your PC.

(Autodesk recommends a minimum of 16Mb of RAM, but be aware that this 
is the basic configuration) 


AutoCAD release 14 for Windows users
------------------------------------

If you receive an error message about a missing or inconsistent driver
file you can manually fix up the acad14.cfg file in the following way:

1.- Make sure that you have left AutoCAD and it is not running.

2.- Open the acad14.cfg file in a text editor of your choice.
    acad14.cfg is an ASCII file so is readable by almost any text
    editor.

3.- Replace every occurrence of the string

      "Hewlett-Packard HP-GL/2 devices, ADI 4.3 - for Autodesk by HP"

    by the string

      "Hewlett-Packard HP-GL/2 devices v4.0, ADI 4.3 - by HP".

    This tells AutoCAD to use the new driver with the associated
    devices.

4.- Save the file and exit the text editor.

You should now be able to start AutoCAD without getting the error
message.

You may want to run "config" again and select "modify" and
"reconfigure" to reconfigure any devices you have installed.
Note that HP LaserJets now support raster images, so you should
reconfigure your LaserJet 4 devices into either "HP LaserJet
(11x17, A3)" or "HP LaserJet (Standard)" which is available with
this driver.


Windows for Workgroups users
----------------------------

Windows for Workgroups users should check they have the latest
versions of operating system files.


Windows NT users
----------------
1.- If you have configured printers to use a specific LPTx port and you
    try to print from AutoCAD using this same port, you may get an error
    message saying that AutoCAD is unable to set up that port.  This is
    because AutoCAD tries to access the hardware directly.  In order to
    avoid this problem there should be no printer configured to use the
    same LPTx port that you want to use from AutoCAD.

3.- How do you plot from AutoCAD 13 in Windows NT, on a plotter that is
    connected to a server?

    a) Go to the DOS command prompt and type:

	net use LPTx "network plotter name" /persistent:yes

    b) Configure your plotter in AutoCAD in the normal way.  When prompted
       for a COM/LPT port number place a dot (.) for none.

    c) While configuring the plotter, go to system parameters, and change
       the default plot file name to c:\<local path>\LPTx.

4.- If the Installer fails to detect previous installation of AutoCAD...

    If you are on Windows NT 4.0 and you have installed AutoCAD under an
    account with administrator privledges, you should also install this
    driver under an account with administrator privledges.  If you don't,
    the installer may fail to detect the location of the AutoCAD
    installation.  You can work around this problem also by entering the
    exact directory location of the AutoCAD installation when you are
    prompted by the installer. 



     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Driver notes: (only for Asian versions)
---------------------------------------

This section describes the environment in which the localized version 
of the AutoCAD driver is supported in the Asian countries.


China
-----
English version of AutoCAD for DOS (r10, r11, r12 and r13), together with 
the ACE layer and the HP English AutoCAD driver for DOS.

English version of AutoCAD for Windows (r12 and r13), together with the 
ACE layer and the HP Chinese AutoCAD driver for Windows. 


Taiwan
------
English version of AutoCAD for DOS (r10 and r11), together with 
the HP English AutoCAD driver for DOS.

Taiwanese version of AutoCAD for DOS (r12 and r13), together with 
the HP Taiwanese AutoCAD driver for DOS.

English version of AutoCAD for Windows r12, together with the HP English
AutoCAD driver for Windows.

Taiwanese version of AutoCAD for Windows r13, together with the HP Taiwanese
AutoCAD driver for Windows.


Korea
-----
English version of AutoCAD for DOS (r10 and r11), together with 
the HP English AutoCAD driver for DOS.

Korean version of AutoCAD for DOS (r12 and r13), together with 
the HP Korean AutoCAD driver for DOS.

English version of AutoCAD for Windows r12, together with the HP English
AutoCAD driver for Windows.

Korean version of AutoCAD for Windows r13, together with the HP Korean
AutoCAD driver for Windows.
