---
title: Extras
layout: index
---


# Distance Extras

This page contains the latest information about Distance, including news, known problems, and material for download (replacement sample projects, Distance add-ons, etc).

If you are having problems with Distance, please check the [problems page](/Distance/bugreport.html).

Unless indicated otherwise, all of the downloads below are packaged as self-extracting archive files. To download an archive file, click on its link. Once it has downloaded, execute the file to unpack it, and then see the readme file for futher instructions.

## General

[Report a bug in Distance](/Distance/bugreport.html)

Downloads, useable with more than one version of Distance. See also the list of [Other Software](othersoftware.html) some of which interface with Distance and the [Distance R packages](R/index.html).

* [Visual interface to activity package](activity)
    - Provides web-based access to the core functionality of the activity package in R.  For use as part of camera trap distance sampling (CTDS) data analysis.
* [MapObjects runtime library](downloads/Mo23rt.EXE) 
    - Library needed for the Design Engine; this is part of the Distance software installation.  However, re-installing MapObjects may alleviate some difficulties experienced by users of the Design Engine.  However, _do not install unless advised to by one of the Distance support team_.  A [documentation file](downloads/MO23Runtime.doc) is also available.
* [DAO database engine](downloads/daosetup.exe) 
    - This archive contains the DAO 3.51 installation package, from Microsoft (about 3MB in size). Re-installing DAO has been found to solve a "Run time error 91" problem that can occur in Distance on some computer configurations. See the known problems list for details. Warning: _do not install unless advised to by one of the Distance support team_.
* [GxHisto - A macro for reproducing the detection function histograms in MS Excel 97](downloads/gxhisto.exe)
    - Contributed by Dr. Tim Gerrodette, Southwest Fisheries Science Center, NMFS.
    - This macro allows you to reproduce the high-resolution detection    function histograms produced by Distance 3.5 and later within Microsoft Excel as MS Charts. You do this by copying the graph data from Distance (by clicking the copy button), pasting it into Excel, and running the macro. Distance already provides the facility to copy the plots as pictures, but these pictures can not then be edited. Using this macro, you are free to change the plot format (colors, axes, etc) as you wish.
    - Note: this macro only works in Excel 97 or later - if you have an earlier version of Excel please contact Dr. Gerrodette (address is in the download's readme).
* [Information and Excel macro for converting data stored as frequency of counts in different distance intervals into format required by Distance](downloads/convert.zip)
    - Contributed by Matt Schlesinger, Aaron Ellingson , Jeremy Lindsell and others.
    - This zip file contains replies to the following email which Matt posted to the distance-sampling list in December 2004.  It also contains an Excel file with a macro for doing the job (by Aaron) and a Word document describing how to do it manually (for another similar data set, by Jeremy)
    - "[...] I'm converting my bird point transect data to Distance format. We recorded birds in 25-m distance categories. The data were entered into MS Access in the following format, to match the data sheet for easy entry (each of these fields separated by commas are columns in the data table): `Site, station, visit, species, 0-25, 25-50, 50-75, 75-100, >100`
    - Each row is a combination of site, station, visit, and species, with the total number of detections within each distance category noted in the appropriate column. [...] Distance requires that each detection be its own row. [...] Does anyone know of a way to convert a format like mine to Distance format easily?"
* Any other ideas?...
    - If you have written a utility program that you think others would find useful in their dealings with Distance we would be happy to publish it here. Please [contact us](/authors.html).

## Running Distance on other operating systems.

### Linux

Although we don't have any direct experience, Distance should run without problems within the emulation software [VMWare](http://www.vmware.com/), [win4lin](http://www.netraverse.com/), [Parallels](http://www.parallels.com/), [VirtualBox](http://www.virtualbox.org/), etc.  For VMWare, note that there is a free version called VMWare player, and if you search the web under something like "Free VMWare" you will find instructions about how to set up operating system images using free software (one site is [http://johnbokma.com/vmware-player/](http://johnbokma.com/vmware-player/)). VirtualBox is opensource and supported by Oracle.  Other possibilities are to use the free emulators [Bochs](http://bochs.sourceforge.net/) (pronounced "box" - slow, apparently) or [QEMU](http://fabrice.bellard.free.fr/qemu/index.html) (with the accelerator module).  For up to date information, try searching the web for "PC Emulators" or "PC Virtualizers".  If you try any of these solutions, please let us know how you get on! We have one report of VirtualBox running Distance 6.0 under Ubuntu platform without trouble.

### Mac

For OS X, many emulators are available - examples include [Parallels](http://www.parallels.com/) and the opensource [VirtualBox](http://www.virtualbox.org/). If you try any of these, then let us know how they work. Parallels (v11) worked fine on OSX releases "Leopard", "Snow Leopard", "Lion", "Mountain Lion", "Mavericks" and "El Capitan" on both PowerPC and Intel Macs (thanks to Jack Lawson for providing this information). Another option, if you have an Intel-based Mac, is to use [Apple's Boot Camp software](http://www.apple.com/support/bootcamp/) to boot into Windows.

### Cross-platform text issues

One caveat (true of all cross-platform transfers) is that users should be careful when creating ASCII text files on other operating systems for use in Distance. They need to have the Windows carriage-return and line-feed characters at the end of each line. There are many ways to ensure this happens, and users who work under multiple operating systems will be well aware of the issue already.

### Running `MCDS.exe` on other platforms

You may want to use Distance command files on the command line using `MCDS.exe` as described in the Distance manual. This can be achieved on Linux and macOS using the Windows emulator [`wine`](https://www.winehq.org/) on the command line. Note that DOS emulators will not work, as Windows DLLs are required. More recent versions of macOS (Catalina/10.15 onwards) have removed 32-bit support, so [`wine32on64`](https://github.com/Gcenx/homebrew-wine) needs to be used.

## Shapefiles, projections and other GIS matters

  * [ESRI Shapefile Technical Description (PDF)](downloads/shapefile.pdf). This is an white paper produced by ESRI describing the internal format of a shapefile.  It also contains some very useful information about how you should order the vertices of a polygon, for example, to create a "clean" shapefile.
  * [Geographic Coordinate Systems and Map Projections (PDF)](downloads/appendixbprojections.pdf). This is an appendix from Samantha Strindberg's PhD thesis (Strindberg 2001). Sam was a PhD student here at the University of St Andrews and developed the methods used in the survey design part of Distance. This appendix gives some background information about geographic coordinate systems and projections: what are they, which should you choose, etc. Hopefully it will be useful for those not familiar with this aspect of GISs.
  * [Spatial data handling in R cheatsheet (performs direct download)](https://github.com/wegmann/RSdocs/blob/master/Cheatsheet/AniMove_refcard.pdf?raw=true) Martin Wegmann maintains a "cheatsheet" for dealing with spatial data in R.


## See also

 * [Other software](othersoftware.html)

