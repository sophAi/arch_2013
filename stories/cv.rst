.. title: Curriculum Vitae (許伯任)
.. slug: cv
.. date: 20141126 11:10:39
.. tags: draft 
.. link: 
.. description: Created at 20130419 13:19:53

.. 請記得加上slug，會以slug名稱產生副檔名為.html的文章
.. 同時，別忘了加上tags喔!

*********************************************
Curriculum Vitae - Po-Jen Hsu / 許伯任
*********************************************

.. 文章起始CONTACT INFORMATION

Name: **Po-Jen Hsu / 許伯任**

Email:   clusterga@gmail.com

Tel:     +886-952-335534

`(Click on me to download the pdf version) <http://sophAi.github.io/arch_2013/files_2013/cv/PoJenHsu_Cv.pdf>`_

`(Chinese version) <http://sophai.github.io/arch_2013/stories/cv_zh.html>`_

_________________________________________________

EDUCATION
----------

**2014**  Ph.D, Molecular Science and Technology, TIGP, Academia Sinica/Physics, National Central University [`1`_-\ `5`_]

**2003**  M.S. in Physics, National Central University [`9`_-\ `11`_]

**2000**  B.S. in Physics, National Central University

_________________________________________________

RESEARCH INTERESTS
------------------

Machine learning
~~~~~~~~~~~~~~~~

* Time series clustering
* Pattern recognition
* Open data mining

Pattern recognition and time series clustering techniques was applied to the mechanistic studying of protein folding and unfolding [`1`_]. Using pattern recognition, the shape of the composing residues of a protein can be converted to multiple time series functions of shape similarity. Therefore, one can perform time series clustering and segmentation analysis to study the correlation between residues, to understand the undergoing mechanism of amyloids forming that are believed to be associated with brain disorders such as Alzhemier's Parkinson's, and Bovine Spongiform Encelphalitis. In the future research, this method will be used to scrutinize signatures from `Open Data`_ such as medical data, earthquake, weather, traffic, economy, particle physics (`CERN Open Data`_) and so on. 

Pattern recognition is also popular in computer vision. To achieve precise and real-time hand gesture control, a histogram-based method with General Purpose GPU (GPGPU) accelerate technique was developed (GestureCV). The goal is to understand how intelligence recognizes objects and makes decisions. More statistical and dynamical methods will be integrated into this system for more general recognition.

High-speed computation
~~~~~~~~~~~~~~~~~~~~~~

* General purpose GPU 
* PC cluster
* Cloud computing

Complexity and veracity are two major issues in Big Data processing. To facilitate this challenging task, one seeks for any possible solution from conventional PC cluster to modern cloud computing. For example, the genetic algorithm can be accelerated more than 10 times by utilizing PC cluster computation (PTMBHGA). Moreover, the GPGPU technique can dramatically boost the performance to more than 100 times (CL-VAF). Ultimately, it is hoped to adopt cloud computing technique such as Hadoop and distributed file system to extend our scope and ability to the Big Data analysis.

Data Visualization
~~~~~~~~~~~~~~~~~~

Data visualization aims to communicate information clearly, efficiently, and interactively to common users using effective visual diagrams. Currently, I'm using numpy and matplotlib as the tools for data representation. In the future, web-based visualization technique such as HTML5 and JavaScript (ex: D3.js) will be implemented.

Open Source Projects
~~~~~~~~~~~~~~~~~~~~

I'm interested in building tool chains from statistical sampling to model simulation. I enjoy programming very much and spent much time in software engineering. Nowadays, smart phone and tablet have equipped powerful CPU and GPU. Most of them are only used for gaming and web browsing. However, I saw the possibility of high-speed computation on these devices. This year I join IT industry to work on GPGPU technique for mobile devices and embedded system. I hope one day these devices can become new computing resources to benefit science and education.

All my programs were published by Open Source licenses, which are listed as follows: 

(**Click on each subtitle to the corresponding GitHub repository**) 

`GestureCV`_
============

*Hand gesture control based on histogram analysis(C++/OpenCL/OpenCV)*

.. image:: ../../arch_2013/files_2013/cv/Hand_Gesture_Program.jpg
   :width: 480
   :target: ../../arch_2013/files_2013/cv/Hand_Gesture_Program.jpg

Framework of GestureCV.

.. youtube:: s4KVkK_wsbQ

Demonstration of GestureCV.

GestureCV combines image filtering and histogram analysis toGestureCV combines image filtering and histogram analysis to accomplish precise real-time hand gesture control on laptop or embedded system. It is a machine learning prototype for computer vision. accomplish precise real-time hand gesture control on laptop or embedded system. It is a machine learning prototype for computer vision.GestureCV combines image filtering and histogram analysis to accomplish precise real-time hand gesture control on laptop or embedded system. It is a machine learning prototype for computer vision.

`CL-VAF`_
=========

*Vector Autocorrelation Function with GPGPU (C++/OpenCL)*

.. image:: ../../arch_2013/files_2013/cv/gpu_performance.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/gpu_performance.png

Performance of CL-VAF. (**click on image to enlarge**)

CL-VAF [`3`_, `4`_, `5`_, `7`_, `8`_] implements GPGPU technique to calculate the autocorrelation function of multi-dimensional vectors.

`MPI-Tools`_
============

*MPICH Tools for PC cluster (Shell Script)*

MPI-Tools allows users to deploy and monitor jobs created by MPICH on PC cluster. It is written in shell script language.

`PTMBHGA`_
==========

*Parallel Tempering Multicanonical Basin-hopping Plus Genetic Algorithm (Fortran/MPICH)*

.. image:: ../../arch_2013/files_2013/cv/ptmbhga.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/ptmbhga.png

Framework of PTMBHGA.

PTMBHGA [`2`_-\ `5`_,\ `9`_-\ `11`_\ ] combines several state-of-art optimization techniques such as genetic algorithm, parallel tempering Monte Carlo method, simulated annealing, basing- hopping method, and multicanonical Monte Carlo method. It is flexible and reliable for searching global optimized result. This program has been used by research groups in Japan and Malaysia.


`PTMD`_
=======

*Parallel Tempering Molecular Dynamics Simulation (Fortran/MPICH)*

.. image:: ../../arch_2013/files_2013/cv/ptmd.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/ptmd.png

Framework of PTMD.

PTMD [`2`_, `4`_-\ `8`_\ ] is designed for model simulation and several statistical analyses including moments, Fourier transformation, and nearest neighbor analysis. It integrates a task schedule system so that users can perform multiple simulations and analyses in parallel.

`D-Tools`_
==========

*Tools for Diffusion Theory (C/C++)*

The D-tools [`3`_] reduces the tedious preparation for diffusion theory calculation. The research was published with Dr. `Arnaldo Rapallo <http://www.ismac.cnr.it/pagine/pagina.aspx?ID=Modelling001&L=IT>`_\ from ISMAC, Italy. 

Other Codes (Mainly matlab and python codes)
============================================

* Time series clustering
* Time series segmentation
* Sliding window algorithm
* Power spectrum density
* Nearest neighbor analysis.

Other experience in Open Source
===============================

Chinese translations of PhET education project in Physics (`EzGo`_, OSSACC, Ministry of Education)

  #. `Davission-Germer Experiment <http://phet.colorado.edu/zh_TW/simulation/davisson-germer>`_
  #. `Stern-Gerlach Experiment <http://phet.colorado.edu/zh_TW/simulation/stern-gerlach>`_
  #. `Quantum Wave Interference <http://phet.colorado.edu/zh_TW/simulation/quantum-wave-interference>`_
  #. `Quantum Tunneling <http://phet.colorado.edu/zh_TW/simulation/quantum-tunneling>`_
  #. `Quantum Bound States <http://phet.colorado.edu/zh_TW/simulation/bound-states>`_
  #. `Covalent Bonds <http://phet.colorado.edu/zh_TW/simulation/covalent-bonds>`_
  #. `Band Structure <http://phet.colorado.edu/zh_TW/simulation/band-structure>`_

_________________________________________________

PROFESSIONAL EXPERIENCE
--------------------------

**2014 - now**  Senior Engineer, Innovation Digital System, System Software Development Division, Hon Hai Precision IND. CO., LTD. --Responsible of Image recognition algorithm, hand gesture control algorithm, HTML5 acceleration (WebCL), GPGPU applications and development of Android input system

**2005 - 2008**  Research assistant in Physics department, National Central University.
--Built and maintained PC clusters and Linux web/mail servers. Built algorithms and models from scratch to simulate chemical and biological materials under statistical mechanics circumstances. [`6`_-\ `8`_]

**2003 - 2005**  Military service

_________________________________________________

PROFESSIONAL FIELD
--------------------

* Computer vision (OpenCV), hand gesture control, and image recognition 
* Applied statistics [`2`_\ ], time series analysis [`1`_\ ], and numerical modeling
* Parallel computing and GPGPU (OpenCL) techniques
* Open Source projects for science and education
* Software management and engineering, SVN/GIT, and UML
* Statistical mechanics, quantum mechanics, chemical physics, applied mathematics, algorithm, and programming language teaching
* Linux/Android input subsystem

_________________________________________________

PROFICIENT IN
--------------

* C++/C, OpenCL, OpenCV
* HTML5/JavaScript, XML, D3.js
* Python, numpy, matplotlib
* Matlab/Octave
* Linux system programming (IPC, thread, socket...)
* Shell script
* Fortran
* Latex
* Regular expression

Award
--------

* `Best Team Presentation Award`_, `4th Hope Meeting`_, 2012, Japan.

Invited talk
--------------
“Open Source in Physics", `International Conference on Open Source 2009`_, Taiwan (`slides`_)

Information of recommendation letters
----------------------------------------

* \ `鄭王曜`_\  教授(中央大學物理系，Email: wycheng@ncu.edu.tw /電話:(03)4227151#65337)
* \ `陳永富`_\  教授(中央大學物理系， Email: yfuchen@cc.ncu.edu.tw /電話:(03)4227151#65375)
* \ `Dr. Arnaldo Rapallo` (ISMAC, Italy. Email: rapallo@ismac.cnr.it)

_________________________________________________


PUBLICATIONS
------------------

(**Click on the title to download the paper**)

.. _1:

1. `Precursory Signatures of Protein Folding/Unfolding: From Time Series Correlation Analysis to Atomistic Mechanisms <http://sophAi.github.io/arch_2013/files_2013/cv/JCP_submitted.pdf>`_, **P. J. Hsu**, S. A. Cheong, and S. K. Lai, J. Chem. Phys. 140, 204905 (2014).

.. _2: 

2. `A new perspective of shape recognition to discover the phase transition of finite-size clusters <http://sophAi.github.io/arch_2013/files_2013/cv/JCC_accepted.pdf>`_, **P. J. Hsu**, J. Comput. Chem. 35, 1082 (2014).

.. _3: 

3. `Peptide dynamics by molecular dynamics and diffusion theory methods with improved basis sets <http://sophAi.github.io/arch_2013/files_2013/cv/JCP_accepted.pdf>`_, **P. J. Hsu**, S. K. Lai, and A. Rapallo, J. Chem. Phys. 140, 104910 (2014).

.. _4: 

4. `Melting behavior of Ag14 cluster: An order parameter by instantaneous normal modes <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/84.pdf>`_,
P. H. Tang, T. M. Wu, **P. J. Hsu**, and S. K. Lai, J. Chem. Phys. 137, 244304 (2012).

.. _5:

5. `Comparative study of cluster Ag17Cu2 by instantaneous normal mode analysis and by isothermal Brownian-type molecular dynamics simulation <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/82.pdf>`_,
P. H. Tang, T. M. Wu, T. W. Yen, S. K. Lai, and **P. J. Hsu**, J. Chem. Phys. 135, 094302 (2011).

.. _6:

6. `Dynamical study of metallic clusters using the statistical method of time series clustering <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/81.pdf>`_,
S. K. Lai, Y. T. Lin, **P. J. Hsu**, and S. A. Cheong, Compt. Phys. Commun. 182, 1013 (2011).

.. _7:

7. `Melting behavior of noble-metal-based bimetallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/78.pdf>`_,
T. W. Yen, **P. J. Hsu**, and S. K. Lai, e-J. Surf. Sci. Nanotech. 7, 149-156 (2009).

.. _8:

8. `Melting scenario in metallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/77.pdf>`_,
**P. J. Hsu**, J. S. Luo, S. K. Lai, J. F. Wax, and J-L Bretonnet, J. Chem. Phys. 129, 194302 (2008).

.. _9:

9. `Structure of bimetallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/71.pdf>`_,
**P. J. Hsu** and S. K. Lai, J. Chem. Phys. 124, 044711 (2006).

.. _10:

10. `Multi-canonical basin-hopping: a new global optimization method for complex systems <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/63.pdf>`_,
L. Zhan, B. Piwowar, W. K. Liu, **P. J. Hsu**, S. K. Lai, and Jeff Z. Y. Chen, J. Chem. Phys. 120, 5536 (2004).

.. _11:

11. `Structures of metallic clusters: mono- and polyvalent metals <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/61.pdf>`_,
S. K. Lai, **P. J. Hsu**, K. L. Wu, W. K. Liu, and M. Iwamatsu, J. Chem. Phys. 117, 10715 (2002).

.. 文章結尾

.. 超連結(URL)目的區

.. _Molecular Science and Technology: http://tigp.iams.sinica.edu.tw/

.. _TIGP: http://tigp.sinica.edu.tw/

.. _National Central University: http://www.phy.ncu.edu.tw/

.. _GestureCV: http://github.com/sophAi/GestureCV

.. _CL-VAF: https://github.com/sophAi/clvaf.git

.. _MPI-Tools: https://github.com/sophAi/mpitool.git

.. _PTMBHGA: https://github.com/sophAi/ptmbhga.git

.. _PTMD: https://github.com/sophAi/ptmd.git

.. _D-Tools: https://github.com/sophAi/dtool.git

.. _TCOM: https://github.com/sophAi/tcom.git

.. _International Conference on Open Source 2009: http://www.slat.org/icos2009/xoops/modules/tinyd0/index.php?id=10

.. _Arnaldo Rapallo: http://www.ismac.cnr.it/pagine/pagina.aspx?ID=Modelling001&L=IT

.. _4th Hope Meeting: http://www.jsps.go.jp/english/e-hope/gaiyou4.html

.. _slides: http://sophAi.github.io/arch_2013/files_2013/cv/icos2009.pdf

.. _EzGo: http://ossacc.moe.edu.tw/uploads/datafile/ezgo7_linux/

.. _Best Team Presentation Award: http://sophAi.github.io/arch_2013/files_2013/cv/hope_award.jpg

.. _鄭王曜: http://www.phy.ncu.edu.tw/?folder=faculty&page=detail.php&pk=271

.. _陳永富: http://www.phy.ncu.edu.tw/?folder=faculty&page=detail.php&pk=270

.. _CERN Open Data: http://opendata.cern.ch/

.. _Open Data: http://www.opendata.tw/
