.. title: Publications - Po-Jen Hsu / 許伯任
.. slug: cv_ref
.. date: 20170303 11:13:24
.. tags: cv
.. link:
.. description: Created at 20130419 13:19:53

.. 請記得加上slug，會以slug名稱產生副檔名為.html的文章
.. 同時，別忘了加上tags喔!

*********************************************
Publications - Po-Jen Hsu 許伯任
*********************************************

.. 文章起始CONTACT INFORMATION

Name: Po-Jen Hsu

Email:   clusterga@gmail.com

Tel:     +886-952-335534


_________________________________________________

PUBLICATIONS
------------------

(**Click on the title to download the paper**)

.. _1:

1. `Exploration of hydrogen bond networks and potential energy surfaces of methanol clusters with a two-stage clustering algorithm <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_12.pdf>`_,
**P. J. Hsu**, K. L. Ho, S. H. Lin, and J. L. Kuo, Phys. Chem. Chem. Phys. 19, 544 (2017).

.. _2:

2. `Precursory Signatures of Protein Folding/Unfolding: From Time Series Correlation Analysis to Atomistic Mechanisms <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_11.pdf>`_,
**P. J. Hsu**, S. A. Cheong, and S. K. Lai, J. Chem. Phys. 140, 204905 (2014).

.. _3:

3. `A new perspective of shape recognition to discover the phase transition of finite-size clusters <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_10.pdf>`_,
**P. J. Hsu**, J. Comput. Chem. 35, 1082 (2014).

.. _4:

4. `Peptide dynamics by molecular dynamics and diffusion theory methods with improved basis sets <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_09.pdf>`_,
**P. J. Hsu**, S. K. Lai, and A. Rapallo, J. Chem. Phys. 140, 104910 (2014).

.. _5:

5. `Melting behavior of Ag14 cluster: An order parameter by instantaneous normal modes <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_08.pdf>`_,
P. H. Tang, T. M. Wu, **P. J. Hsu**, and S. K. Lai, J. Chem. Phys. 137, 244304 (2012).

.. _6:

6. `Comparative study of cluster Ag17Cu2 by instantaneous normal mode analysis and by isothermal Brownian-type molecular dynamics simulation <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_07.pdf>`_,
P. H. Tang, T. M. Wu, T. W. Yen, S. K. Lai, and **P. J. Hsu**, J. Chem. Phys. 135, 094302 (2011).

.. _7:

7. `Dynamical study of metallic clusters using the statistical method of time series clustering <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_06.pdf>`_,
S. K. Lai, Y. T. Lin, **P. J. Hsu**, and S. A. Cheong, Compt. Phys. Commun. 182, 1013 (2011).

.. _8:

8. `Melting behavior of noble-metal-based bimetallic clusters <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_05.pdf>`_,
T. W. Yen, **P. J. Hsu**, and S. K. Lai, e-J. Surf. Sci. Nanotech. 7, 149-156 (2009).

.. _9:

9. `Melting scenario in metallic clusters <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_04.pdf>`_,
**P. J. Hsu**, J. S. Luo, S. K. Lai, J. F. Wax, and J-L Bretonnet, J. Chem. Phys. 129, 194302 (2008).

.. _10:

10. `Structure of bimetallic clusters <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_03.pdf>`_,
**P. J. Hsu** and S. K. Lai, J. Chem. Phys. 124, 044711 (2006).

.. _11:

11. `Multi-canonical basin-hopping: a new global optimization method for complex systems <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_02.pdf>`_,
L. Zhan, B. Piwowar, W. K. Liu, **P. J. Hsu**, S. K. Lai, and Jeff Z. Y. Chen, J. Chem. Phys. 120, 5536 (2004).

.. _12:

12. `Structures of metallic clusters: mono- and polyvalent metals <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_01.pdf>`_,
S. K. Lai, **P. J. Hsu**, K. L. Wu, W. K. Liu, and M. Iwamatsu, J. Chem. Phys. 117, 10715 (2002).

_________________________________________________

PERSONAL OPEN SOURCE PROJECTS
-----------------------------

Click on each title to access the corresponding GitHub repository and download the source code.

`TSCA`_
=======

*Two-stage Clustering Algorithm (Python/SQLite)*

TSCA [`1`_] archives molecular structures into SQLite databases and performs a two-stage clustering method based on the forming shape and the bonded networks of the molecules to trim down the number of isomers. This algorithm has been proven efficient in various hydrogen bonded systems such as methanol, alcohol, and ammonia clusters.


`PTMBHGA`_
==========

*Parallel Tempering Multicanonical Basin-hopping Plus Genetic Algorithm (Fortran/MPICH)*

PTMBHGA [`3`_-\ `6`_, \ `10`_-\ `12`_\ ] combines several state-of-the-art optimization techniques such as the genetic algorithm, parallel tempering Monte Carlo method, simulated annealing, basing-hopping method, and multicanonical Monte Carlo method. It is flexible and reliable for searching global strucutre in cluster system. This program has been adopted by research groups in Japan and Malaysia.


`PMD`_
=======

*Parallel Molecular Dynamics Simulation (Fortran/MPICH)*

PMD [`3`_, `5`_-\ `9`_\ ] is designed for model simulation and several statistical analysis including moments, Fourier transformation, and nearest neighbor analysis. It integrates a task schedule system so that users can perform multiple simulations and analysis in parallel.


`CL-VAF`_
=========

*Vector Autocorrelation Function with GPGPU (C++/OpenCL)*

CL-VAF [`4`_, `5`_, `6`_, `8`_, `9`_] utilizes the power of GPU (Graphical Processing Unit) to accelerate the autocorrelation calculation of multi-dimensional vectors.

`GestureCV`_
============

*Hand gesture control based on histogram analysis (C++/OpenCL/OpenCV)*

GestureCV combines image filtering and histogram analysis to accomplish precise real-time hand gesture control on laptops or embedded systems. It is a machine learning prototype for computer vision.

`g09tools`_
===========

*Tools for submission and recovering of Gaussian software (Shell Script)*

g09tools [`1`_] will scan all the Gaussian input files in a folder and construct the qsub/bsub script for submitting to the PBS system. It will automatically recognize the status of the Gaussian job (failed or running). If failed jobs are detected, it will retrieve the last SCF snapshot and continue the SCF steps. It is written in shell script language.


`grotools`_
===========

*Tools for Gromacs software (Shell Script)*

grotools [`3`_, `4`_] helps to run Gromacs software with pdb file easier. It is written in shell script language.


`MPI-Tool`_
============

*MPICH utility for PC cluster (Shell Script)*

MPI-Tool allows users to deploy and monitor jobs created by MPICH on PC clusters. It is written in shell script language.


`D-Tool`_
==========

*A utility for Mode-coupling Diffusion Theory (C/C++)*

D-Tool [`4`_] reduces tedious preparation for mode-coupling theory calculation. The work was published with Dr. `Arnaldo Rapallo`_ from ISMAC, Italy.


OTHERS
------

Chinese translations of PhET education project in Physics (`EzGo`_, OSSACC, Ministry of Education)

* `Davission-Germer Experiment <http://phet.colorado.edu/zh_TW/simulation/davisson-germer>`_
* `Stern-Gerlach Experiment <http://phet.colorado.edu/zh_TW/simulation/stern-gerlach>`_
* `Quantum Wave Interference <http://phet.colorado.edu/zh_TW/simulation/quantum-wave-interference>`_
* `Quantum Tunneling <http://phet.colorado.edu/zh_TW/simulation/quantum-tunneling>`_
* `Quantum Bound States <http://phet.colorado.edu/zh_TW/simulation/bound-states>`_
* `Covalent Bonds <http://phet.colorado.edu/zh_TW/simulation/covalent-bonds>`_
* `Band Structure <http://phet.colorado.edu/zh_TW/simulation/band-structure>`_

_________________________________________________

.. 文章結尾

.. 超連結(URL)目的區

.. _StatPhys-Taiwan-2016: http://www.phys.cts.nthu.edu.tw/actnews/content.php?Sn=295

.. _Molecular Science and Technology: http://tigp.iams.sinica.edu.tw/

.. _TIGP: http://tigp.sinica.edu.tw/

.. _National Central University: http://www.phy.ncu.edu.tw/

.. _GestureCV: http://github.com/sophAi/GestureCV

.. _CL-VAF: https://github.com/sophAi/clvaf

.. _grotools: https://github.com/sophAi/grotools

.. _g09tools: https://github.com/sophAi/g09tools

.. _TSCA: https://github.com/sophAi/TSCA

.. _MPI-Tool: https://github.com/sophAi/mpitool

.. _PTMBHGA: https://github.com/sophAi/ptmbhga

.. _PMD: https://github.com/sophAi/ptmd

.. _D-Tool: https://github.com/sophAi/dtool

.. _TCOM: https://github.com/sophAi/tcom

.. _International Conference on Open Source 2009: https://blog.lxde.org/?tag=icos2009

.. _Arnaldo Rapallo: http://www.ismac.cnr.it/laboratories/modelling/?lang=en

.. _Siew Ann Cheong: https://www.linkedin.com/pub/siew-ann-cheong/22/384/4b4

.. _San-Kiong Lai: http://www.phy.ncu.edu.tw/wp/faculty/賴山強-s-k-lai

.. _4th Hope Meeting: http://www.jsps.go.jp/english/e-hope/gaiyou4.html

.. _download slides: http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_icos2009.pdf

.. _download pycon slides: https://drive.google.com/file/d/0B-rXMt0bOKG8aTA3QWpOeURJTVU/edit

.. _PyCon 2015: https://tw.pycon.org/2015apac/zh/schedule/

.. _EzGo: http://ossacc.moe.edu.tw/uploads/datafile/ezgo7_linux/

.. _Best Team Presentation Award: http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_award.jpg

.. _鄭王曜: http://www.phy.ncu.edu.tw/english.php?folder=faculty&page=detail.php&pk=271

.. _陳永富: http://www.phy.ncu.edu.tw/english.php?folder=faculty&page=detail.php&pk=270

.. _CERN Open Data: http://opendata.cern.ch/

.. _Open Data: http://www.opendata.tw/

.. _link 1: http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_TIGP_certificate.jpg

.. _link 2: http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_PhD_certificate_en.jpg

.. _link: http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_PhD_transcript.jpg

.. _D3.js: http://en.wikipedia.org/wiki/D3.js

.. _NumPy: http://en.wikipedia.org/wiki/NumPy

.. _Matplotlib: http://en.wikipedia.org/wiki/Matplotlib

.. _OpenCL: http://en.wikipedia.org/wiki/OpenCL

.. _WebCL: http://en.wikipedia.org/wiki/WebCL

.. _OpenCV: http://en.wikipedia.org/wiki/OpenCV

.. _GSL: http://en.wikipedia.org/wiki/GNU_Scientific_Library

.. _SVN: http://en.wikipedia.org/wiki/Apache_Subversion

.. _Git: http://en.wikipedia.org/wiki/Git_(software)

.. _XML: http://en.wikipedia.org/wiki/XML

.. _UML: http://en.wikipedia.org/wiki/Unified_Modeling_Language

.. _GPU: http://en.wikipedia.org/wiki/Graphics_processing_unit

.. _GPGPU: http://en.wikipedia.org/wiki/General-purpose_computing_on_graphics_processing_units

.. _Hadoop: http://en.wikipedia.org/wiki/Apache_Hadoop

.. _Molecular Science and Technology: http://tigp.iams.sinica.edu.tw/

.. _OpenMPI: https://en.wikipedia.org/wiki/Open_MPI

.. _MPICH: https://en.wikipedia.org/wiki/MPICH

.. _libxml2: https://en.wikipedia.org/wiki/Libxml2

.. _TIGP: http://tigp.sinica.edu.tw/

.. _thesis: http://140.113.39.130/cgi-bin/gs32/ncugsweb.cgi?o=dncucdr&s=id=%22GC972402012%22.&searchmode=basic

.. _download thesis: http://140.113.39.130/cgi-bin/gs32/ncugsweb.cgi?o=dncucdr&s=id=%22GC972402012%22.&searchmode=basic

.. _Arduino: http://www.arduino.cc/

.. _Diffusion Equation: http://en.wikipedia.org/wiki/Diffusion_equation

.. _Rouse-Zimm: http://en.wikipedia.org/wiki/Rouse_model

.. _GNU Make: https://en.wikipedia.org/wiki/Make_(software)#Modern_versions

.. _CMake: https://en.wikipedia.org/wiki/CMake

.. _CLIQ website: http://www.phy.ncu.edu.tw/~cplx/facilities.html

.. _CLIQ webmail: http://cliq.phy.ncu.edu.tw/cgi-bin/openwebmail/openwebmail.pl
