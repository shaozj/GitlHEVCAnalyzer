What is Gitl HEVC Analyzer
==========================

![logo](https://github.com/lheric/GitlHEVCAnalyzer/blob/master/screenshots/logo.png?raw=true)

Gitl HEVC/H.265 Analyzer is an open-source tool for bitstream analysis for HEVC/H.265 .

It is released under Apache License 2.0. In addition, it's **NOT for commercial use**. If you want to use it for commercial purpose, please contact us. If you are not using it to develop weapons, produce or sell illegal drugs, and if you are not a terrorist, we will give your a commercial version for **free**.

**If you are using our analyzer in your paper, please add a footnote or reference to our work**

Current building status:  [![Build Status](https://travis-ci.org/lheric/GitlHEVCAnalyzer.png?branch=master)](https://travis-ci.org/lheric/GitlHEVCAnalyzer)

Looking for **binary**?

(**If the binary is unstable on your system, please compile it from the source code**)

Windows (64 bit):

<a href="https://sourceforge.net/projects/gtilhevcanalyzer/">https://sourceforge.net/projects/gtilhevcanalyzer/</a>

For linux users, please compile the source code

If you find any bugs, you are welcomed to open  new issues.


Why Gitl HEVC Analyzer
======================

First, all the commercial HEVC analyzers are too expensive.

Second, we need to draw additional grphics on the analysis results. It supports custom filters. In fact, all the features are implemented via custom filters.

Documents
=========

Program structures (coming soon)

How to write a custom filter (coming soon)

Screenshot
==========
Windows (Dark theme):
![Win](https://github.com/lheric/GitlHEVCAnalyzer/blob/master/screenshots/screenshoot_win.png?raw=true)

Linux (Default theme):
![Linux](https://github.com/lheric/GitlHEVCAnalyzer/blob/master/screenshots/screenshoot_linux.png?raw=true)

Features
========

Support YUV420 (8bit) bitstream.

For historical reasons, besides formal HEVC bitstream, it also supports bitstreams generated by older HM encoders (HM-4.0, HM-5.2, HM-10.0 and HM-12.0).

<ul>
    <li>Custom Plugins Support</li>
    <li>Zoom In/Out Details</li>
    <li>Predition Type Display</li>
    <li>Coding Unit (CU) Display</li>
    <li>Predition Unit (PU) Display</li>
    <li>Transform Unit (TU) Display</li>
    <li>Motion Vectors (MV) Display</li>
    <li>Intra Mode (Angular, DC, Planar) Display</li>    
</ul>

<a href="http://gitl.sysu.edu.cn">Intelligent Information Processing Lab</a> 

Road Map
========
- [X] Frames Bit Heatmap Filter
- [X] Frame Timeline
- [ ] Slice Display
- [ ] Tile Display
- [ ] GOP Structure Graph
- [ ] 10 Bit YUV Support
- [ ] Bitsteam Comparison 

How To Build
============

Written in C++ with Qt5 (c++11 support required)
You should get and install **Qt 5.1.0 or higher**.

1.  Clone this repository.
```bash
git clone https://github.com/lheric/GitlHEVCAnalyzer.git GitlHEVCAnalyzer
```

2.  Init & update the submodules.
```bash
cd GitlHEVCAnalyzer
git submodule update --init --recursive
git submodule update --recursive
```

3a. Build on linux:
```bash
qmake -qt=qt5 GitlHEVCAnalyzer.pro -r "CONFIG+=Release"
make
```

3b. Build on windows:
```bash
qmake GitlHEVCAnalyzer.pro -r "CONFIG+=Release"
make
```

Instead of the building on the command line , Qt Creator is supported. Clone this project and its submodules, then open `GitlHEVCAnalyzer.pro` in Qt Creator.

Contact Us
============
<a href="http://gitl.sysu.edu.cn">Intelligent Information Processing Lab</a>

School of Software, Sun Yat-sen University, Guangzhou, P.R.China

Author:
Huang Li (李璜)

lihuang55555@gmail.com


Supervised by Prof. Hongyang CHAO

Hongyang Chao (朝红阳)

isschhy@mail.sysu.edu.cn

School of Software

Sun Yat-sen University
