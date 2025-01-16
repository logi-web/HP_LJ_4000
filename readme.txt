*********************************************************************
Product Registration for the HP LaserJet 4000 series printers.
*********************************************************************

Register your Hewlett-Packard LaserJet 4000 series printer on the
world wide web by visiting the following URL:

      //www.hp.com/go/lj4000_register



*********************************************************************
   HINTS for INSTALLING SOFTWARE
        
*********************************************************************

---------------------------------------------------------------------
Virus Checking Software

Disable all virus checkers before starting the installation process.
Re-enable the virus checkers after the installation process is
complete.



*********************************************************************
                      
   HINTS for PRINTING SOFTWARE
        
*********************************************************************


---------------------------------------------------------------------
Online Help

Online help is provided with the HP LaserJet 4000 Printing System. 
This help can be accessed from the help buttons on dialog boxes of
the  various HP LaserJet 4000 Printing System components (drivers or
HP Toolbox).


---------------------------------------------------------------------
Windows Notepad or Cardfile Characters Missing

If you are printing with either Notepad or Cardfile and the first few 
characters are missing from the left side of the page, you can
correct this using one of the following methods:  1. Change the left
margin setting in the printer driver by selecting Page Setup from the
File menu, changing the left margin setting to 0.5 in., and printing
the document again. 2. Change the printer resolution from 600 dpi to
300 dpi. (PCL 5e Driver only). If you change resolution, remember to
change it back to 600 dpi when you are finished printing.


---------------------------------------------------------------------
Graphics, Memory Errors, and Print Performance

If you encounter printing difficulties, memory errors, or slow 
performance with any application, refer to the online Help topic,
"Common Print Problems," for additional information. 


---------------------------------------------------------------------
Text Compatibility with Earlier HP LaserJet Printers

If a text incompatibility exists between a document printed with
another HP LaserJet printer and the HP LaserJet 4000 printer, try the
following:

  *  First, if using the PCL 5e Printer Driver, go to the Print
     Quality tab and select "Manual" and "Truetype as Bitmaps." 
  *  If the incompatibility still exists, and you are using 
     the PCL 5e Printer Driver, change the print optimization
     setting to 300 DPI Printing and print the document again.
     If you are using the PCL 6 Printer Driver and the previous
     document was printed with the PCL 5e Printer Driver, change
     to the PCL 5e Printer Driver. If the PCL 5e Printer Driver
     is not installed, run the HP Printing System installation.


---------------------------------------------------------------------
CorelDRAW Printing Performance

The options below are made available to assist you in improving
print speed. Print performance, however, is largely dependent on
information in the graphics document being printed. 

1.  Print Performance (PCL 5e Printer Driver only)

For best printing performance in CorelDRAW, if you have selected 
HP-GL/2, it is recommended that you change the Graphics Mode to
either Automatic or Raster.

2.  CorelDRAW 3.0 - Improve graphics performance. 
    a) Open the CORELDRW.INI file with a text editor.
       The CORELDRW.INI file is in the DRAW subdirectory for
       CorelDRAW 3.0b or later 
       (e.g., c:\corel30\coreldrw\draw\coreldrw.ini).
    b) Go to the section labeled: [CDrawConfig]. 
    c) At the end of this section, enter the following line (exactly
       as shown): UseClippingForFills=0
       (If the line: UseClippingForFills=3 is present, please change
       it to read: UseClippingForFills=0)
    d) Save and close the CORELDRW.INI file. 
    e) Restart CorelDRAW. 

3.  CorelDRAW 4.0 and 5.0 - Improve graphics and scanned image 
    printing performance. 
    a) Open the CORELDRW.INI file with a text editor.
       The CORELDRW.INI file is found in the COREL40\CONFIG
       subdirectory for CorelDRAW 4.0 and 5.0
      (e.g., c:\corel40\config\coreldrw.ini).
    b) Go the section labeled:[Config]
    c) At the end of this section, enter the following line (exactly
       as shown): UseClippingForFills=0
       (If the line: UseClippingForFills=3 is present, please change
       it to read: UseClippingForFills=0)
    d) Save and close the CORELDRW.INI file.
    e) Restart CorelDRAW.

The following setting affects raster graphics only. 

    a) Open the CORELPRN.INI file with a text editor.
       The CORELPRN.INI file is also located in the CONFIG
       sub-directory. 
    b) Go to the section labeled:   [Config]
    c) Find the following line:     DumpEntireBitmap=0 
       Change it to read:           DumpEntireBitmap=1 
    d) Save and close the CORELPRN.INI file.
    e) RESTART CorelDRAW. 
                 
    Changing this entry from 0 to 1 allows CorelDRAW to send raster 
    data in blocks rather than line by line. This should improve 
    processing time for graphic-intense files and improve
    performance. 

CorelDRAW 6.0 and 7.0 - Improve graphics and scanned image
printing performance.

a) Launch CorelDRAW.  Place an object on the page and click File
   Print. Select the Options button and then the Options Tab.
b) Go to the section named Special Settings:
c) From the drop down list of options select Fill Clipping.
d) Change the setting from Use Driver Clipping For Fills to
   Use Software Clipping For Fills.
e) Select OK to close out of the Options dialog, Cancel to close
   out of the print dialog.
f) Close the CorelDRAW application and re-start CorelDRAW.

The following setting affects raster graphics only.

a) Launch CorelDRAW.  Place an object on the page and click File
   Print. Select the Options button and then the Options Tab.
b) Go to the section named Special Settings:
c) From the drop down list of options select Bitmap Printing.
d) Change the setting from Output in 64K Chunks to
   Output Entire Bitmap.
e) Select OK to close out of the Options dialog, Select OK to print
   or Cancel to close out of the print dialog.  The application
   does not have to be re-started.

---------------------------------------------------------------------
Additional Memory Installed in the Printer

If you have installed additional memory or removed memory from the 
printer, the printer driver should be updated manually. To identify 
the exact amount of memory, do one of the following:

  * If you are using the PostScript Printer Driver, print a self test
    page and refer to the Total Memory value. To set the information
    in the driver, open the driver, click on the "Device Options",
    and then enter the amount of memory into the "Available printer
    memory" box.



*********************************************************************
   Windows 3.1/3.11 PS Driver
*********************************************************************

---------------------------------------------------------------------
Resolutions
The Windows 3.1/3.11 driver does not support multiple resolutions in
one printer instance.  The default is 600 dpi and that is the driver
that will be installed with the Printing System installer.  To use
other resolutions, you will have to install multiple instances of the
same driver.  To do this, open the Control Panel and double click on
Printers.  Click Add>>.  Click Install.  Browse to the installation
disk and into the directory WIN3X\<country>\DISK1.  The available
printers will be listed with the supported resolution indicated at
the end of the printer name.  Select the printer instance you want to
install and click OK.

---------------------------------------------------------------------
Paper Source Names
The paper source names in the driver do not correspond to the names
on the printer.

Upper Tray = Tray 1
Middle Tray = Tray 2
Lower Tray = Tray 3
Large Capacity = Tray 4

---------------------------------------------------------------------
Custom Paper Sizes
To print on a custom paper size, setup the size first in the driver.
To do this, select User Defined Size in the Paper Size drop down
list.  In the dialog that appears, enter the width and height.
Notice that the units are in fractions of inches and millimeters, so
for a 3x5 inch paper size, enter 300 x 500.  If the application you
are using supports custom sizes in its Page Setup or Page Layout,
setup a corresponding size in the application.  Select either Auto
Select or Upper Tray in the Paper Source drop down list.  Place the
custom size paper in Tray 1 and print the document.  If you do not
put the paper in Tray 1 before you print, the printer may pull paper
from a lower tray.  If you select Manual Feed with a custom paper
size, you will get the default resolution set on the printer, not
the resolution specified in the driver.


---------------------------------------------------------------------
Adobe Acrobat (Windows 3.1x only)
For EPS files, Acrobat uses the Number of Copies setting specified
for the entire document within Acrobat. This overrides the PS
printer driver setting of 1 for the Number of Copies option for EPS
files, and might lead to unexpected printing results.

Workaround: This problem will be corrected in a future release of
Acrobat; in the meantime, set the Number of Copies option in Acrobat
to 1.




*********************************************************************
   Windows 95 PS Driver
*********************************************************************

---------------------------------------------------------------------
Data Format Setting
The driver's default setting for Data format is ASCII Data option.
ASCII Data option sends all data to the printer in Adobe
Communication Protocol. ASCII Data format allows the file to print on
any printer.

For faster printing, if your printer is connected directly to your
computer via a serial or parallel port and your printer supports a
binary data format, or if you intend to print to a printer connected
over an AppleTalk or Ethernet, you may want to change the Data
format setting from ASCII to one of the binary data formats that is
applicable to your setting. 

---------------------------------------------------------------------
Sending Error Handler to Printer With Reduced Memory
If your printer is low in memory, the error handler might not be able
to print complete messages if error conditions occur.

Workaround: Either add more memory to your printer or disable the
error handler by turning off the Print PostScript Error Information
option in the PostScript properties dialog box.


---------------------------------------------------------------------
Print jobs with multiple page sizes and specific paper trays set will
result in only the first page's paper size and tray selection to be
sent to the printer.  This will cause all document pages to be
printed on the same paper size and tray selection.  

Workaround:  To work properly AutoSelect must be picked for the Paper
Source or a Custom paper size must be chosen.  

---------------------------------------------------------------------
Printing Colored Text
Some applications will print colored as text rather than in grayscale
when the output device is a black and white printer.  

Workaround:  Use a color PS driver or the PCL driver.

---------------------------------------------------------------------
Type 1 Bold Font Imperfections
The driver provides an emboldening feature for outline fonts (Type 1)
that do not have a native bold version, such as Zapf Dingbats. The
emboldening process is inexact and might produce slight typographic
imperfections.

Workaround: To eliminate typographic imperfections, choose a Type 1
font family that has a native bold face.

---------------------------------------------------------------------
Printing TrueType Fonts
Some characters of TrueType fonts, such as the o in the Economicals
font, might not print correctly. This problem is due to problems with
the fonts themselves.

Workaround: To eliminate font imperfections, you might want to use
another font.

---------------------------------------------------------------------
Specifying Available Printer Memory
The PS printer driver allows you to specify any value for the
Available Printer Memory option in the Device Options properties
dialog box. If you specify a value outside the range of your printer,
very large files might be generated, printing performance might be
poor, or printing might fail. 

Workaround: Normally, the default value the PS printer driver
supplies is adequate for most needs. If you need to change this
value, however, make sure the value you set for this option falls
within the available memory specifications of your printer. You can
get printer memory information by printing a test page from the
General properties dialog box.

---------------------------------------------------------------------
Margin Conversion Discrepancies
When you set margins in the Unprintable Area dialog box, you specify
a number that the PostScript printer driver uses in its calculations
of unprintable area. In these calculations, the driver rounds off
the numeric value you provide for the unprintable area to its nearest
point equivalent. Because of this, you might notice small
discrepancies between the numbers you specified and the numbers that
appear in the fields after you click OK in the Unprintable Area
dialog box.  The value .20 is always reset to .19.

Workaround: None.

---------------------------------------------------------------------
On occasion patterns will appear much smaller on the printed output
than the screen (e.g., PowerPoint v7.0).  This is a driver defect
demonstrated by certain use of patterns in some applications.  

Workaround:  Try printing at a lower resolution or use the PCL driver.



---------------------------------------------------------------------
Adobe PageMaker 5.0
Windows metafiles printed from Adobe PageMaker 5.0 in landscape
orientation are cut off on the right side. PageMaker 5.0 clips at
portrait width. 

Workaround: Do not use landscape orientation when printing Windows
metafiles from Adobe PageMaker 5.0, or use a later version of
PageMaker.

---------------------------------------------------------------------
PageMaker v6.0:
The user must install the PPD into the PageMaker specified
directory to obtain access to printer features.  The PPD should be
located in the Windows/System directory and also on the installation
disks.  NOTE: When printer specific features are accessed, the
default PageMaker uses is to use the printers default setting, rather
than the PPD specified default setting.  Thus the user may need to
change multiple features to gain access to all of the drivers
capabilities.

---------------------------------------------------------------------
AmiPro 3.1 
When you select a block of justified text and apply the double
underline style to it, AmiPro 3.1 documents do not print fully
underlined. 

Workaround:  Use single underlined text, not double-underlined, or
try double-underlining one line of text at a time.

---------------------------------------------------------------------
Designer
Printing multiple master fonts from the Designer application causes
PostScript errors. 

Workaround: Do not use multiple master fonts with the Designer
            application.

---------------------------------------------------------------------
FileMakerPro 2.0: Documents with integrated graphics print out
                  incorrectly.
 
Workaround: Upgrade to FileMakerPro 2.1.

---------------------------------------------------------------------
FrameMaker 5.0
Printing text with integrated graphics from the FrameMaker 5.0
application results in a PostScript error.

Workaround: Upgrade to FrameMaker 5.1 or 6.0.

---------------------------------------------------------------------
Lotus 1-2-3: cannot always calculate the text placement of
             inverted, rotated text. Text might be missing or
             incorrectly placed in a printout.
             This problem occurs rarely.

Workaround: None.

---------------------------------------------------------------------
Microsoft Excel 5.0
You might encounter some problems printing from Excel 5.0: Print
settings specified from within Excel 5.0 are ignored when the
document is printed.

Workaround: Specify the print settings from the Printers folder only.

---------------------------------------------------------------------
Microsoft Word
If you change driver settings within the Microsoft Word Page Setup
dialog box and select an option that conflicts with your current
configuration, the PS printer driver cannot inform you of the
conflict. 

Also in the Page Setup dialog box of Microsoft Word 7.0, Word
replaces the custom paper names that you specify with its own fixed
names for custom paper; the custom paper settings you have set are
still valid and the document prints correctly.

---------------------------------------------------------------------
Persuasion
Persuasion does not save the n-up layout values that you select in
the Paper properties dialog box.

Workaround: You must reselect the layout setting each time a document
is printed.

---------------------------------------------------------------------
Photoshop 3.04
If a conflict exists in the data format selections made within
Photoshop 3.04 and in the driver, any file printed from Photoshop
3.04 results in a PostScript error. 

Workaround: If your printer is connected over a pure binary channel,
such as AppleTalk, and you wish to print in binary format, choose the
Pure Binary Data option in the Data Format menu (the Data Format menu
is in the Advanced PostScript Options dialog box, which you open by
clicking Advanced in the PostScript properties dialog box); then
choose binary format in Photoshop 3.04. If you choose any other
binary option in the driver (Binary Communications Protocol or Tagged
Binary Communications Protocol), you must set the format to ASCII in
Photoshop 3.04 to avoid a PostScript error; in this case, your
document does not print in binary mode.

---------------------------------------------------------------------
Driver Feature Incompatibility
Sometimes an application might be incompatible with the PS printer
driver. With those applications, you cannot use certain PS printer
driver features. For example, you cannot use the following driver
features with these applications:

Mirror Image:
Acrobat 2.0
CorelDRAW! 6.0
Exchange 2.0
Illustrator 4.0

Negative Image:
PageMaker 5.0

N-up Format:
Acrobat 2.0
Excel 5.0
Exchange 2.0
PageMaker 5.0

Rotated Landscape:
Acrobat 2.0
Exchange 2.0
PageMaker 5.0
WordPerfect 6.1

Scaling:
Acrobat 2.0
AmiPro 3.1
CorelDRAW! 6.0
Exchange 2.0
FrameMaker 4.0
PageMaker 5.0

Workaround: Do not use these PS printer driver features when running
the corresponding applications. Upgrading to more recent versions of
some of these applications, such as Acrobat 2.1, allows you to use
these features.



*********************************************************************
   Windows NT Application Interactions with PostScript
*********************************************************************
Application Specific Issues:

General Application Information:
If a customer does not like the print quality produced with certain
applications, it may be due to the application overriding the
printers default halftone.  The work around is to “use printers
halftone” in the application configuration if supported or to set
the levels of gray to “enhanced” in the drivers advanced features
menu.

The NT driver does not support custom paper sizes.  A customer can
print custom sizes by formatting their job using one of the standard
paper sizes then adjusting the margins until the desired position is
obtained.

The Windows NT driver shows many more paper sizes than supported by
the printer.  These additional paper sizes are selectable in an
application but will be mapped to the closest next larger paper size
and the job formatted for the requested paper size.

On occasion patterns will appear much smaller on the printed output
than the screen (e.g., PowerPoint v7.0).  This is a driver defect
demonstrated by certain use of patterns in some applications.  There
is no work around for PostScript, use the PCL driver to fix the
problem.

The default driver is generally selected when an application is run.
The default driver will be selected even when a document composed with
another driver is opened.  This is the behavior of some applications
under Windows NT and has been the behavior of HP’s solutions under NT,
however, this is different than the Windows 95 Adobe solution.

Some applications will by-pass the PostScript driver that may cause
the printer to receive a non terminated job resulting in a job timeout.
Using the supplied PostScript separator page (Pscript.sep) can
minimize the impact of these applications on other jobs.  This file can
be set as the separator page in the Windows NT print manager by
selecting the printer in the settings menu the selecting the Separator
Page under the general tab under the printers properties page.

---------------------------------------------------------------------
Windows NT Wordpad:
   Wordpad and the driver can get out of sync in print orientation.
   For example, if the user sets orientation in the driver different
   than the Wordpad setting, the document prints in the driver
   orientation, but is formatted for the application orientation.
   This is easy to work around by setting the orientation in the
   application page setup rather than the driver.

---------------------------------------------------------------------
Microsoft Publisher 97:
   Fill patterns do not print in PostScript.
   The workaround is to use the PCL driver.

---------------------------------------------------------------------
PageMaker v6.0:
   The user must install the PPD into the PageMaker specified
   directory to obtain access to printer features.  NOTE: When
   printer specific features are accessed, the default PageMaker
   uses is to use the printers default setting, rather than the PPD
   specified default setting.  Thus the user may need to change
   multiple features to gain access to all of the drivers
   capabilities.

---------------------------------------------------------------------
Corel v6.0 Applications:
   Corel v6.0 is not officially supported on Windows NT 4.0, thus the
   user may run into problems like we have seen with Corel Dream in
   which bitmap images do not print correctly in PostScript using the
   standard Pscript driver.  The images are banded with overlapping
   data producing an incomplete image.

---------------------------------------------------------------------
Corel WordPerfect v7.0 and Corel Presentations v7.0:
   These applications do not provide access to the advanced driver
   features tab when the driver is accessed within the application.
   Set the advanced features through the printer’s settings “document
   defaults” menu item, selected from the “Start, Settings” menu
   item.

---------------------------------------------------------------------
Corel v7 Applications:
   The Corel v7 applications do not send the drivers job boundary
   commands (e.g., PJL) to the printer in Windows NT.  Thus
   resolution, economode and job separator commands will not be sent
   to the printer (the customer will receive the printer’s default
   settings).  The job boundary issue will cause a data received
   message on the control panel until another job is sent or until
   the job timeout period has elapsed.  This becomes more of an issue
   when the customer is attempting to use printer collation.  The
   printer will not complete the job until the job timeout time has
   elapsed.  The work around is to use the PCL driver.

---------------------------------------------------------------------
Adobe Acrobat v3.0:
   Acrobat does not send PJL commands to the printer thus resolution,
   language switching, job boundaries and economode are not
   supported.

   Acrobat v3.0 does not use the resolution or copy count set in the
   driver or via the application’s print dialogue box.  The user gets
   one copy at the printers default resolution.  This is also true of
   PCL and XL.

---------------------------------------------------------------------
Micrografx Picture Publisher v6.0:
   This application generates it own PostScript, the default
   configuration produces grainy images.  The application must be
   configured to produce higher resolution image data.

---------------------------------------------------------------------
Lotus 1-2-3:
   Lotus prints color text as black rather than gray scale when the
   output device is monochrome.  If the customer wants gray scale
   text, use the PCL driver or a color PostScript driver.

---------------------------------------------------------------------
Microsoft Excel:
   Excel performs formatting of the page based upon the printer’s
   resolution, thus producing rounding differences for different
   resolutions.  The application does correctly represent page
   breaks, however, the user should be aware that page breaks can
   change based on resolution if the customer formats their margins
   to be exactly the width of the individual Excel columns.

   Excel prints color text as black rather than gray scale when the
   output device is monochrome.  If the customer wants gray scale
   text, use the PCL driver or a color PostScript driver.

---------------------------------------------------------------------
Visual Basic in Excel:
   Visual basic within Excel can generate device dependent PostScript
   code resulting in line width differences when the printer’s
   resolution is modified.  The work around is to use PCL.

---------------------------------------------------------------------
Microsoft Word v7.0:
   MS Word can produce text that overlaps if the user uses several
   spaces to position text to a fixed position (e.g., a border).
   This is fixed with Word 97.  You can also correct this problem by
   setting position via tabs or using PCL.

---------------------------------------------------------------------
Miscellaneous Driver Related Issues:
   The PostScript imageable area is slightly smaller than previous
   products.  PostScript now uses the same imageable area as PCL.

---------------------------------------------------------------------
Pages per Sheet:
   If multiple pages per sheet place the pages on the sheet in the
   wrong order, it is probably due to an orientation mismatch between
   the page orientation and the pages per sheet orientation.  As a
   rule of thumb the user should select a portrait pages per sheet
   orientation for portrait data and landscape for landscape data.

   Multiple copies using duplex or multiple pages per sheet can
   result in individual copies of the job not being separated.
   This occurs if application collation is enabled.  The work around
   is to use printer collation in the driver and turn off application
   collation.

   Adobe Acrobat places multiple pages on the same frame, use only
   the one page per sheet setting or use the PCL driver.

   QuarkXpress v3.3 places multiple pages on the same frame, use
   only one page per sheet setting or use the PCL driver.

---------------------------------------------------------------------
Negative:
   The PostScript driver performs negative images on every other
   page with one page per sheet setting with the PostScript Page
   Independence set to the default value of off.  The work around
   is for the user to turn Page Independence on.  NOTE: Page
   Independence on instructs the driver to not send PJL commands
   that set the resolution, control economode or mark job
   boundaries.

   The negative image capability is not compatibility with multiple
   pages per sheet setting.

---------------------------------------------------------------------
Mirror Image:
   The PostScript driver shifts the image on the printed page by
   approximately 0.38 of an inch. The workaround is to reduce the
   left and right margins in the application by .38 of an inch. 




*********************************************************************
   TECHNICAL ASSISTANCE
*********************************************************************

Some of the services below are provided for the United States only.
Similar services to those listed below are available in other
countries.  See your printer's User's Guide or call your local
authorized HP dealer.


CUSTOMER SUPPORT

For free customer support during the Warranty Period, call
(208) 323-2551 (US only) Monday through Friday, 6:00 a.m. to
6:00 p.m., Mountain Time.
Have your serial number ready when calling.

INTERNET

Anonymous FTP library service is available world-wide for
around-the-clock-access to drivers and technical support information
for HP peripheral and computer products.  Please note that paths may
change without notice.  Access the Internet or FTP address and use
the menus to locate the software or support of your choice.  

•	URL for Software and Support: http://www.hp.com/go/cposupport
•	URL for Access HP: http://www.hp.com

•	FTP address: ftp.hp.com
		Login: anonymous
		Password: your Internet name (or user identification)

HP SOFTWARE AND SUPPORT SERVICES - ADDITIONAL INFORMATION

Refer to your printer user's guide for additional methods of
obtaining software and support information, such as printer driver
distribution centers, other online services, fax services, and other
online support.


*********************************************************************
   LEGAL STATEMENTS
*********************************************************************


TRADEMARK NOTICES

MS-DOS, Windows, and MS Windows are registered trademarks of
   Microsoft Corp.
Novell and NetWare are U.S. registered trademarks of Novell, Inc.
IBM and OS/2 are registered trademarks of IBM Corporation.
Macintosh is a registered trademark of Apple Computer, Inc.
TrueType is a registered trademark of Apple Computer, Inc.
Intellifont is a registered trademark of AGFA Compugraphic,
   a division of Miles Corporation.
Adobe, PageMaker, and PostScript are registered trademarks of
   Adobe Systems, Incorporated.
CorelDRAW! is a registered trademark of Corel Corporation.


SOFTWARE LICENSE AND COPYRIGHT

Information provided in this document and software called the
HP LaserJet 4000 Series Printing System is provided "as is."
No implied warranties of merchantability and or fitness for a
particular purpose are given.

The HP LaserJet 4000 Series Printing System may be copied and
distributed only to users of an HP LaserJet 4000 Series printers.
All files on the CD must be copied without modification.  All
components of the HP LaserJet 4000 Series Printing System must be
distributed together.  The HP LaserJet 4000 Series Printing
System may not be distributed for profit.

Copyright (c) 1990, 1991, 1992, 1993, 1994, 1995, 1996, 1997
   Hewlett-Packard Company.
Copyright (c) 1985, 1986, 1987, 1988, 1989, 1990 Microsoft Corp.
Copyright (c) 1988, 1989, Aldus Co.
All Rights Reserved.

*********************************************************************
