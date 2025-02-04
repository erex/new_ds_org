---
generator: Microsoft Word 11.0.0000;
operator: Len Thomas
---

**[Distance 7.5 Release 2]{.underline}**

**[Release Notes - February 2023]{.underline}**

*Contents*

Installation Notes

Upgrading from previous versions of Distance

Uninstalling Distance

Distance-sampling email list

Current restrictions

New features, resolved issues and known problems

Reporting problems

Appendix 1: Files Added During Installation

**Installation Notes**

*System Requirements for Distance 7.5*

***Operating System and Hardware Requirements***

Any modern desktop PC will have no problem installing and running
Distance 7.5. It requires about 90MB of space on your hard drive, and
either Windows 7, 8 or 10 operating systems. (Distance will likely also
run under older versions of Windows operating systems; however this is
no longer actively supported. If you are using a legacy operating
system, be aware that the practical minimum hardware requirements are a
Pentium II Processor, 48MB RAM, 800x600 SVGA monitor with 256 colors.)

***R Statistical Software***

Three analysis engines and the simulation engine in Distance 7 are
implemented as libraries in the free statistical software R. These are
the Mark Recapture Distance Sampling (mrds), Density Surface Modelling
(dsm), Multi-Analysis Distance Sampling (mads) and the Distance Sampling
Simulations (dsims) libraries. If you would like to run any of these
engines, you must install R software on your computer first. You can
download R from the R Project web site, http://www.r-project.org/. You
need the base precompiled binary distribution for Windows.

*The R libraries in this version of Distance (7.5 release 2) were tested
and compiled using R version 4.2.2. You will need to install this
version of R and point Distance to it in the R Options after selecting
the Preferences option from the Tools menu.*

Please note that R is under very active development, and new versions
are released quite frequently. Unfortunately, new versions are sometimes
not compatible with libraries compiled in old versions. We will endeavor
to test our libraries with each new version as it appears, and update
are libraries as required. We will post any information we have about
compatibility with new versions on the Distance-sampling email
discussion list (see below), so please check there for latest
information.

You can download and install R after you have installed Distance, and
you can run Distance without having R installed - but you will get an
error message if you try to run the MRDS, DSM, MA analysis engines or
the simulation engine without R.

For more information about the R-Distance link, see the Distance online
help, Chapter 7. There you will find a topic \"R Statistical Software\".

***Windows Script 5.6***

If you are trying to run Distance with a legacy version of Windows
(before Windows Vista) you may need to install Windows Script, if it is
not already on your machine. The Distance installation program contains
a copy of the English language verion of Windows Script 5.6, and you
have the option to install this as part of the program setup. If you are
using a non-English version of Windows, you will probably want to
download and install the version of Windows Script appropriate for your
language \-- you can get this from http://www.microsoft.com/scripting/.
If you have already installed the appropriate version of Windows Script
on your computer, then you should say \"No\" when the Distance setup
program asks you if you want to install it\'s version.

**PDF file Reader**

The Distance User\'s Guide is also available in Adobe PDF format. To
read this file (which is installed in the Distance/Help directory), you
need software capable of reading PDF files. One example is Adobe Acrobat
reader, available for free from http://www.adobe.com, but other free
software is available.

*Running Distance under other operating systems*

To run Distance under non-Windows operating systems, a Windows emulator
is required. For some tips, see the section on \"Running Distance on
other operating systems\" at
http://distancesampling.org/distanceextras.html.

*Running Distance in extended character systems*

If you use an extended character operating system (e.g., Chinese,
Japanese or Korean language Windows) then you need to make the following
change to the program preferences before you start using the program.
Once you have installed Distance:

1\. Start Distance

2\. From the menu, choose Tools \| Preferences\...

3\. Click on the General tab. Un-tick the box \"Store results in
compressed format in project databases\"

4\. Click OK.

You need to make this change because by default Distance compresses the
results from analyses when it stores them in project databases, and at
present it cannot decode these results on extended character operating
systems.

*Installing Distance under Windows*

The Distance setup program has a filename of the form
d\[x\]release\[y\].exe, where \[x\] is derived from the version number
and y is the release number. Double-click on this file to run it. You
are then guided through the installation. If you have an older operating
system, you may be asked to re-boot again early in the installation
process and then restart the install. You may also be asked to reboot
after install has finished. You need to have administrator privileges to
install Distance.

Once Distance is installed, you can run Distance 7 from the Programs \|
Distance 7 folder off the Start menu on your windows Taskbar.

A list of the files added by Distance installation is given in Appendix
1.

***Problems with Install***

Problems encountered when installing Distance are recorded here:
https://github.com/DistanceDevelopment/distance-bugs

The main installation issues encountered include conflicts with
antivirus software and problems opening dlls. Conflicts with antivirus
software can be resolved by temporarily disabling the antivirus software
prior to installation. Issues relating to dll conflicts are more
complicated, please contact us at distance@st-andrews.ac.uk and we will
be happy to try to help you resolve the problem. We now build an
alternative installer to try to get round these issues.

Another common issue is a warning produced by Windows Defender:

Windows protected your PC

Microsoft Defender SmartScreen prevented an unrecognized app from

starting. Running this app might put your PC at risk.

[More info]{.underline}

We are working on a resolution to this problem, but in the meantime
please be assured that Distance is perfectly safe to install, and the
following is a work-around to the error message.

· Click on the [More info]{.underline} link.

· You should see a button Run anyway.

· Click on the Run anyway button and the installation should proceed as
normal.

If you are having a problem that is not listed there, please (1) check
your computer meets the minimum requirements (above); (2) check the
archives of the distance-sampling discussion list (see below); (3) look
at the file C:\\Program Files (x86)\\Distance 7\\Install.log to see if
it gives you any clues as to the problem; (4) contact the program
authors by email: distance@st-andrews.ac.uk.

*Sample Projects*

Information on the sample projects is given in Chapter 2 of the online
help.

**Upgrading from previous versions of Distance**

Distance 7.5 will install over any previous Distance 7.x installations,
it is not necessary to remove these installations prior to installing
Distance 7.5. Distance 7.5 will register itself to open .dst files when
you double-click on them. If you open a Distance project created in a
previous version, you will be asked if you wish to upgrade it, and if
you say \"Yes\", Distance will perform the upgrade automatically.

When upgrading Distance you should also upgrade to the recommended
version of R. Failing to do so may mean that you continue using old
versions of the R packages or the newer R packages may not work in the
older version of R. Note that, to ensure that Distance installs the new
R packages on the first run of an analysis that uses one of the R-based
analysis engines, please take the following steps:

· Choose Tools \| Preferences \| R Options

· Tick the box that says Re-install analysis / simulation engine
libraries to original versions on the next run.

Note also that to successfully upgrade the R packages when you run an
analysis, all other instances of R need to be closed.

You are advised to re-run all analyses as the analysis engines are
improved with each iteration of the software.

If you have a copy of Distance 6, 5, 4 or 3.5 on your machine, you
don\'t have to uninstall it before installing Distance 7. Distance 7
will install into a different directory, and you can carry on using both
the older and new version of the software if you wish. However, please
note that if you upgrade a Distance project using Distance 7, you will
not be able to open it in any of the previous versions. Should you wish
to do this, you should copy the project before upgrading, so you can
open the old files in the old version. One convenient way to copy a
project from within Distance is to use File \| Export project.

Please let us know if you have any problems transitioning to the new
version of Distance.

**Uninstalling Distance**

To uninstall Distance, click on the Add/Remove Programs icon in the
Windows Control Panel. Choose Distance 7 from the list and click the
Add/Remove button. During the removal process, you will be asked whether
you want to remove shared components. Press \"Yes to All\". The install
program may not be able to remove all of the folders under C:\\Program
Files\\Distance7\\ if you have changed any files in them (e.g., by
creating new projects in \\Sample projects). In this case you will have
to remove these folders manually after the installation has finished.

**Distance-sampling email discussion list**

The purpose of this list is to promote the sharing of ideas and
information among researchers and practitioners interested in distance
sampling techniques. It is a relatively low-volume list, and has been
running since 1998, first as a JISCmail list, but more recently as a
Google Group.

Suitable topics for posting include: questions about survey design and
analysis, new methodological developments, use of software tools
(program Distance and other software), news about upcoming meetings,
workshops and conferences where distance methods will be discussed, jobs
in distance sampling-related fields.

You can browse the list without joining, by navigating to
groups.google.com and searching for the group distance-sampling If you
have a Google account, you can join via that; alternatively, you can
send a blank email to distance-sampling+subscribe@googlegroups. In
response, you will receive a message with a link button to \"Join this
group\", please follow the instructions. Once you have completed the
steps you will receive a second E-mail asking you again to confirm via
clicking on the \"Join this group\" button. You should then be informed
that you have been successfully subscribed. See
http://distancesampling.org/distancelist.html for further information.

Posts from the old JISCmail mailing list are archived on the Google
Group. Please check the archive of previous messages before posting!

**Current restrictions for Distance 7.5 Release 2**

MCDS Analysis Engine

Maximum number of covariates and factor levels is listed in the manual,
under "Limitations"

When covariates are specified, only half-normal and hazard-rate key
functions allowed

Cannot force the fitted function to be monotonic decreasing

When cluster size is a covariate, stratified analyses are not allowed

Cannot have non-factor covariate value -9999.

MRDS Analysis Engine

Ignores units conversion specified in the Units tab of the Data Filter

MA Analysis Engine

Line transect surveys only

Single observer

Ignores units conversion specified in the Units tab of the Data Filter

Simulation Engine

Line and point transect surveys excluding adjusted angle and equal angle
zig zag designs

Single observer

Only takes the truncation distance from Data Filter (binned data can be
generated in dsims R package)

Minus sampling only

All units must be the same for region, design and detection function

Strata must have unique names/labels

Doesn\'t support data-linked study region

**New features, resolved issues and known problems**

Below is a summary of new features and resolved issues in each recent
version of Distance. For an up to date list, and a list of known
problems, please visit
https://github.com/DistanceDevelopment/distance-bugs

Distance 7.5 Release 2 - Uses latest version of R (4.2.2) with updated
versions of dssd, dsims, Distance and mrds which have various bug fixes.
A fix in dsims now allows for stratum level designs within simulations
at the global level.

Distance 7.5 Release 1 - Uses latest version of R (4.2.1) with updated
versions of mrds, dsm and mads which have various bug fixes. In
addition, the R package DSsim has been replaced with dsims. Includes an
additional example project on the analysis of point transect removal
method data. Fixed bug relating to renaming a new map before you have
opened it.

Distance 7.4 Release 2 - Uses R version of 4.1.2. This release has an
important bug fix to correct the field names stored in the survey
definition for cluster size, object, observer and detected. Anyone using
these fields with projects created in Distance 7.4 release 1 should
check they are correctly specified within the survey definition.

Distance 7.4 Release 1 - Uses latest version of R (4.1.2) with updated
versions of mrds, dsm, DSsim and mads which have various bug fixes.

Distance 7.3 Release 2 - Uses latest version of R (4.0.1) with updated
versions of mrds, dsm, DSsim and mads which have various bug fixes.

Distance 7.3 Release 1 - Addition of a shape import wizard. Bug fixes in
simulation engine. Uses latest version of R (3.5.1) with updated
versions of dsm and DSsim.

Distance 7.2 Release 1 - Mrds and dsm analyses can now be performed for
point transects as well as line transects. Uses latest version of R
(3.5.0) with updated versions of mrds, dsm and DSsim.

Distance 7.1 Release 1 - Uses latest version of R (3.4.1); all R
packages updated. New dsm analytical variance calculation, concurvity
plot and prediction plot using ggplot2 package. Simulations now support
populations that occur in clusters and other individual level
covariates.

Distance 7.0 Release 1 - the public release following the trial of beta
4 during workshops. In addition, we have added an alternative variance
calculation option in dsm and point transect designs have been added to
the simulation engine. The R packages mrds and dsm have also been
upgraded.

Distance 7.0 Beta 4 - now implements designs (generating multiple
surveys) in the simulation engine. Fixes dsm bugs: rqgam.check is only
called when appropriate, gam.check has been added to output for all dsm
models, alpha value for confidence intervals is now passed to the R
library. It relies on the latest version or R 3.3.1 and installs
packages built under this version of R.

Distance 7.0 Beta 3 - relies on the latest version or R 3.2.2 and
installs packages built under this version of R. This seems to fix a
strange bug with dsm variance calculations when an error message was
being generated because object appeared to have missing components.

Distance 7.0 Beta 2 - provides a major bug fix to the design engine.
Distance 7.0 Alpha 1 and Distance 7.0 Beta 1 were both using the
Distance 6 design properties component. If you have Distance 6 installed
you would not have noticed any problems in Distance 7.0. There have been
no updates to the design engine and so everything would have been
functioning correctly if you succeeded in loading the design inputs
page.

Distance 7.0 Beta 1

Here\'s a brief list of new features, resolved issues and known problems
in Distance 7.0 Beta 1, relative to 7.0 Alpha:

General Interface Known Problems

\- About button does not work for Windows 7

\- Designs and Simulations will not run if region or strata names that
they rely on are changed.

MA Engine

An option to specify which field contains species codes has been added

The \'cv\' bug in covariate uncertainty has been fixed

Covariate uncertainty on multiple covariates no longer causes an error

Note that the MA engine requires that the MRDS analysis object exist in
the workspace so the option to remove these objects must be switched off

R packages (mads, mrds, dsm and DSsim) have been updated to latest
versions and compiled under R 3.2.2

See NEWS file in the relevant packages for further information of
changes and/or bug fixes

Here\'s a brief list of new features, resolved issues and known problems
in Distance 7.0, relative to 6.2:

We have made 2 major additions, the multi-analysis (MA) engine and the
simulation engine. The MA analysis engine deals with unidentified
sightings, covariate uncertainty and model uncertainty. The simulation
engine allows you to try out different designs and see how they perform
for your particular study.

**Reporting problems**

To report a new problem, please visit
https://github.com/DistanceDevelopment/distance-bugs and click the \'New
Issue\' button or E-mail us at distance@st-andrews.ac.uk.

**Appendix 1: Files added during Distance 7 Installation**

Note - if older versions of these files are already present, they will
be overwritten. If newer versions are already present, they will not be
changed. (An exception to this is RichEd32.dll, which caused some
incompatibility problems in test installations. This file will only be
installed if one is not present on the target system.) If you selected
the backup option during Setup, backups of all overwritten files will be
stored in the BACKUP subdirectory, off the Distance 7 program directory.
A log of all files installed is kept in the program directory in the
file install.log.

**Common Files \\ Data Dynamics folder**

Actbar2.ocx

**Common files \\ ESRI**

Mo20.ocx

AF20.dll

Shape20.dll

pe81.dll

sg81.dll

mtch.dll

JetTable20.dll

**Microsoft \\ Shared Tools \\ DAO**

Dao2535.tlb

Dao250.dll

Jettable20.dll

Msjet35.dll

Msjint35.dll

Msjter35.dll

Msrd2x35.dll

dbajet32.dll

**Windows System 32 folder**

Asycfilt.dll

Comcat.dll

Comctl32.ocx

Comdlg32.ocx

Expsrv.dll

Mfc42.dll

Msvbvm60.dll

Msvcirt.dll

Msvcp60.dll

Msvcrt.dll

Msvcrt40.dll

mtch.dll

Oleaut32.dll

Oledlg.dll

OlePro32.dll

Riched32.dll

Scrrun.dll

Stdole2.tlb

vb5db.dll

vbar332.dll

vbscript.dll

VsFlex7d.ocx

ccrpdbs6.dll

tab32x30.ocx

mschrt20.ocx

richtx32.ocx

dwAXExtn.dll

Dwsdes32.dll

D7Zip.dll

PolarZip.ocx

PolarZipSpan.dll

RichEd32.dll

Splitter.ocx

**Program Files (x86) \\ Distance7**

Ec.exe

DistanceProject.ico

Distance.exe

D7DbEng.dll

CDlg.dll

CTmr.dll

CSDesc.ocx

LLine.ocx

LogStr.dll

LogWin.ocx

SList.ocx

PrjParams.dll

D7Map.ocx

D7Legend.ocx

DistIni.mdb

ID7NEng.dll

D7NEH.exe

D7NSvr.dll

D7NEIUtil.dll

D7CDSNEI.dll

D7MRDSNEI.dll

D7DSMNEI.dll

D7MANEI.dll

D7SIMNEI.dll

MCDS.exe

D7DesNEI.dll

D7DesEng.dll

D7SvyNEI.dll

D7DFPrp.ocx

D7MDPrp.ocx

D7CDSPrp.ocx

D7MRDSPrp.ocx

D7MAPrp.ocx

D7SIMPrp

D7DSMPrp.ocx

D7DesPrp.ocx

D7SvyPrp.ocx

D7DesDet.ocx

D7SPWiz.dll

DeIDWiz.dll

DistanceLogo.jpg

ReadMe.rtf

support.r

dsm.support.r

mrds.support.r

mads.support.r

dssim.support.r

**Program Files (x86) / Distance / Help**

distance.chm

distance.pdf

Sponsors.rtf

Authors.rtf

DataEntryIntroduction.rtf

DataEntryGlobal.rtf

DataEntryStratum.rtf

DataEntryObservation.rtf

DataEntryFinished.rtf

TipOfTheDay.txt

**Program Files (x86) / Distance / Sample Projects**

\[a number of sample project files\]

**Program Files (x86) / Distance / RPackages**

Copies of all the packages required by the Distance engines that use R.
