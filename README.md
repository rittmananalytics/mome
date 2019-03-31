
![MOME Project](https://rittmananalytics.com/s/momeproject.png)

# Welcome to The Official MOME Development Site

_01-04-2019: Today we’re proud to bring you MOME 1.0.0. There are some big improvements to SunPlus SPG240/SPG280 audio emulation, Cognos Powerplay cube aggregation and initial support for Oracle Financial Analyzer database write-back_

## What is MOME? 
MOME is a framework for emulating multi-dimensional Online Analytical Processing ("MOLAP") engines, 4GL programming languages and the servers and OLAP applications that ran on those engines.

## The MOME Project

MOME's purpose is to preserve decades of multi-dimensional MOLAP engine and software history. As analytical processing technology continues to rush forward, MOME prevents this important "vintage" technology from being lost and forgotten. This is achieved by documenting the MOLAP engine, its multi-dimensional storage format and 4GL query languages, along with the software and sample databases for those engines such as Microsoft OLAP Services 7.0 AdventureWorks. 

Over time, MOME (originally stood for Multiple OLAP Machine Emulator) absorbed the sister-project MESS (Multi-dimensional Engine Super System), so MOME now documents a wide variety of (mostly vintage) MOLAP, Relational OLAP ("ROLAP") and now Hybrid OLAP "HOLAP" engines in addition to the MOLAP engines and desktop applications that were its initial focus.

### Common Universal Binary Engine

The Common Universal Binary Engine ("CUBE") core coordinates the emulation of several common MOLAP engine features at the same time such as indexed lookups, 4GL language parsing and pre-aggregation of leaf-level data. These features are virtualized so MOME acts as a software layer between the original MOLAP 4GL and MDX language  and the virtualized engine that MOME runs in. MOME supports arbitrary dimension sizes, numbers of measures and aggregation hierarchies. 

![MOME Emulator Architecture](https://rittmananalytics.com/s/mome_architecture.png)

Individual MOLAP engines are specified by  _drivers_  which take the form of  [C preprocessor](https://en.wikipedia.org/wiki/C_preprocessor "C preprocessor")  [macros](https://en.wikipedia.org/wiki/Macro_(computer_science) "Macro (computer science)"). These drivers specify the individual engine features to be emulated and how they communicate with each other. 

![Layered Drivers and Hypervisor Model](https://rittmananalytics.com/s/layers.png)

By virtualizing and layering MOLAP functionality in this manner it is now possible to run 4GL commands from one engine to run on another; for example, enabling advanced planning and budgeting applications such as Oracle Express Financial Analyzer and Express Objects to run on Microsoft OLAP Services 7. 

### What MOLAP Engines are Supported?

The initial release of MOME supports the following MOLAP engines and server software:

![Supported MOLAP Engines](https://rittmananalytics.com/s/systems.png)

### Where Can I Download MOLAP Application ROMs?

![ROM Downloads](https://rittmananalytics.com/s/roms2.png)

# M.O.M.E. Homebrew Hardware Projects

MOME can run on many different platforms such as [Windows](http://en.wikipedia.org/wiki/Windows), [Unix](http://en.wikipedia.org/wiki/Unix), [OS X](http://en.wikipedia.org/wiki/OS_X) etc. but by simply analyzing your emulated cubes on a desktop computer it lacks the look and feel of the original office arcade hardware.

![enter image description here](https://rittmananalytics.com/s/retrohardware.png)

An Arcade Cabinet conversion into a MOME Cabinet consists of:  
  
-   removing the original proprietary electronic game board (PCB) inside a cabinet,
-   replacing it with a computer (a PC) and
-   interfacing it (display, controls, sound etc.)
-   flashing required MOLAP engine drivers and application software into a game cartridge
-   connecting it to a printer

Note that you must legally own the original MOLAP engine hardware and applications that you use with MOME.

# Moving to the Cloud?

No hardware! No problem! Discoverer Cloud Service and EPB Cloud Service are available again for just today - 1st April 2019

- [Discover Cloud Service (2018)](https://twitter.com/markrittman/status/980422422330560512)
- [Enterprise Planning & Budgeting Cloud (2018)](https://twitter.com/markrittman/status/980592163707936768)

# License

The MOME project as a whole is distributed under the terms of the  [GNU General Public License, version 2](http://opensource.org/licenses/GPL-2.0)  or later (GPL-2.0+), since it contains code made available under multiple GPL-compatible licenses. A great majority of files (over 90% including core files) are under the  [BSD-3-Clause License](http://opensource.org/licenses/BSD-3-Clause)  and we would encourage new contributors to distribute files under this license.

[![](https://camo.githubusercontent.com/d9f2a52ccb094aecca865c7614750675ddf80fdb/687474703a2f2f6f70656e736f757263652e6f72672f74726164656d61726b732f6f70656e736f757263652f4f53492d417070726f7665642d4c6963656e73652d313030783133372e706e67)](http://opensource.org/licenses/GPL-2.0)

```
Copyright (C) 1997-2019  MOMEDev and contributors

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.

