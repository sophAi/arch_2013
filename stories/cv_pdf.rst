.. title: Curriculum Vitae - Po-Jen Hsu / 許伯任
.. slug: cv_pdf
.. date: 20170303 11:14:40
.. tags: cv
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

`(Click here to see the on-line version) <http://sophai.github.io/arch_2013/stories/cv.html>`_

_________________________________________________

EDUCATION
----------

**2014**: Ph.D., `Molecular Science and Technology`_, `TIGP`_, Academia Sinica/Physics, National Central University. Supervised by Dr. `Siew Ann Cheong`_, Dr. `Arnaldo Rapallo`_, and Dr. `San-Kiong Lai`_ (primary `thesis`_ supervisor) [`1`_-\ `5`_].

**2003**: M.S. in Physics, National Central University [`9`_-\ `11`_]

**2000**: B.S. in Physics, National Central University

_________________________________________________

RESEARCH INTERESTS
------------------

Machine Learning
~~~~~~~~~~~~~~~~

* Time series clustering [`1`_, `6`_]
* Pattern recognition [`1`_, `2`_]
* Open data mining

Pattern recognition and time series clustering techniques were applied to the mechanistic study of protein folding and unfolding [`1`_]. Using pattern recognition, the shape of the composing residues of a protein can be converted into multiple time series functions of shape similarity. Therefore, one can perform time series clustering and segmentation analysis to study the correlation between residues, in order to understand the underlying mechanism of amyloid formation that are believed to be associated with brain disorders such as Alzheimer's disease, Parkinson's disease, and Bovine Spongiform Encephalitis. In future research this method will be used to scrutinize signatures from `Open Data`_ such as medical data, earthquakes, weather, traffic, economy, and particle physics data (`CERN Open Data`_).

.. figure:: ../../arch_2013/files_2013/cv/time_series_analysis.png
   :width: 900
   :target: ../../arch_2013/files_2013/cv/time_series_analysis.png

   **Applied time series analysis and shape recognition tecniques to molecular biology.**

Pattern recognition is also popular in computer vision. To achieve precise and real-time hand gesture control, a histogram-based method with graphics processing units (`GPU`_) acceleration technique was developed (`GestureCV`_). The goal is to understand how intelligence recognizes objects and makes decisions. More statistical and dynamical methods will be integrated into this system for more general recognition.

High-speed Computation
~~~~~~~~~~~~~~~~~~~~~~

* General-purpose computing on graphics processing units (`GPGPU`_) [`2`_, `4`_, `5`_, `7`_, `8`_]
* PC cluster [`1`_-\ `11`_]
* Cloud computing

Complexity and veracity are two major issues in Big Data processing. To facilitate this challenging task, one seeks for any possible solution from conventional PC clustering to modern cloud computing. For example, a time series analysis can be accelerated by more than 10 times by utilizing PC cluster computation (`PTMD`_). Moreover, the `GPGPU`_ technique can dramatically boost the performance to more than 100 times (`CL-VAF`_). Ultimately it is hoped to adopt cloud computing techniques such as `Hadoop`_ and a distributed file system to extend our scope and ability for Big Data analysis.

Data Visualization
~~~~~~~~~~~~~~~~~~

Data visualization aims to communicate information clearly, efficiently, and interactively to common users using effective visual diagrams. Currently, I'm using `NumPy`_ and `Matplotlib`_ as the tools for data representation. In the future, web-based visualization technique such as HTML5 and JavaScript (ex: `D3.js`_) will be implemented.

.. figure:: ../../arch_2013/files_2013/cv/D3_beta.png
   :width: 900
   :target: ../../arch_2013/files_2013/cv/D3_beta.png

.. figure:: ../../arch_2013/files_2013/cv/D3_alpha.png
   :width: 900
   :target: ../../arch_2013/files_2013/cv/D3_alpha.png

   **Visualization of strong (red dashed) and weak (blue dashed) correlations of the time series clustering results [1].**

(`Click here to see the D3.js demonstration`_)

_________________________________________________

OPEN SOURCE PROJECTS
~~~~~~~~~~~~~~~~~~~~~

I'm interested in building tool chains from statistical sampling to model simulation. I enjoy programming very much and have spent a lot of time in software engineering. Smart phones and tablets are currently equipped with powerful CPUs and GPUs, but most of them are only used for gaming and web browsing. However, I saw the possibility of high-speed computation on these devices. This year I joined the IT industry to work on `GPGPU`_ techniques for mobile devices and embedded systems. I hope that one day these devices can become new computing resources to benefit science and education.

All my programs were published by Open Source licenses, which are listed as follows:

(**Click on each subtitle to view the source code repository on GitHub**)

`GestureCV`_
============

*Hand gesture control based on histogram analysis (C++/OpenCL/OpenCV)*

GestureCV combines image filtering and histogram analysis to accomplish precise real-time hand gesture control on laptops or embedded systems. It is a machine learning prototype for computer vision.


.. figure:: ../../arch_2013/files_2013/cv/Hand_Gesture_Program.png
   :width: 1280
   :target: ../../arch_2013/files_2013/cv/Hand_Gesture_Program.png

   **Framework of GestureCV.**

.. figure:: ../../arch_2013/files_2013/cv/Hand_Gesture_Demo.png
   :width: 1150
   :target: ../../arch_2013/files_2013/cv/Hand_Gesture_Demo.png

   **Application switcher and presentation software control.**

(`Click here to view the demonstration on YouTube`_)

`CL-VAF`_
=========

*Vector Autocorrelation Function with GPGPU (C++/OpenCL)*

CL-VAF [`3`_, `4`_, `5`_, `7`_, `8`_] implements GPGPU techniques to calculate the autocorrelation function of multi-dimensional vectors.

.. figure:: ../../arch_2013/files_2013/cv/gpu_performance.png
   :width: 1024
   :target: ../../arch_2013/files_2013/cv/gpu_performance.png

   **Performance of CL-VAF.**


`MPI-Tool`_
============

*MPICH utility for PC cluster (Shell Script)*

MPI-Tool allows users to deploy and monitor jobs created by MPICH on PC clusters. It is written in shell script language.

`PTMBHGA`_
==========

*Parallel Tempering Multicanonical Basin-hopping Plus Genetic Algorithm (Fortran/MPICH)*

.. figure:: ../../arch_2013/files_2013/cv/ptmbhga.png
   :width: 1024
   :target: ../../arch_2013/files_2013/cv/ptmbhga.png

   **Framework of PTMBHGA.**

PTMBHGA [`2`_-\ `5`_, \ `9`_-\ `11`_\ ] combines several state-of-the-art optimization techniques such as the genetic algorithm, parallel tempering Monte Carlo method, simulated annealing, basing-hopping method, and the multicanonical Monte Carlo method. It is flexible and reliable for searching global optimized results. This program has been used by research groups in Japan and Malaysia.


`PTMD`_
=======

*Parallel Tempering Molecular Dynamics Simulation (Fortran/MPICH)*

.. figure:: ../../arch_2013/files_2013/cv/ptmd.png
   :width: 1024
   :target: ../../arch_2013/files_2013/cv/ptmd.png

   **Framework of PTMD.**

PTMD [`2`_, `4`_-\ `8`_\ ] is designed for model simulation and several statistical analyses including moments, Fourier transformation, and nearest neighbor analysis. It integrates a task schedule system so that users can perform multiple simulations and analyses in parallel.

`D-Tool`_
==========

*A utility for Mode-coupling Diffusion Theory (C/C++)*

D-Tool [`3`_] reduces tedious preparation for diffusion theory calculation. The research was published with Dr. `Arnaldo Rapallo`_ from ISMAC, Italy.

Matlab and Python codes
========================

* Time Series Clustering Method [`1`_, `6`_]
* Time Series Segmentation Method [`1`_]
* Sliding Window Method [`1`_, `6`_]
* Pattern Recognition Method [`1`_, `2`_]
* Power Spectrum Density Calculation [`4`_, `5`_, `7`_, `8`_]
* Nearest Neighbor Analysis [`6`_]
* Auto-correlation Calculation [`3`_-\ `5`_, `7`_, `8`_]

Others
=======

Chinese translations of PhET education project in Physics (`EzGo`_, OSSACC, Ministry of Education)

* `Davission-Germer Experiment <http://phet.colorado.edu/zh_TW/simulation/davisson-germer>`_
* `Stern-Gerlach Experiment <http://phet.colorado.edu/zh_TW/simulation/stern-gerlach>`_
* `Quantum Wave Interference <http://phet.colorado.edu/zh_TW/simulation/quantum-wave-interference>`_
* `Quantum Tunneling <http://phet.colorado.edu/zh_TW/simulation/quantum-tunneling>`_
* `Quantum Bound States <http://phet.colorado.edu/zh_TW/simulation/bound-states>`_
* `Covalent Bonds <http://phet.colorado.edu/zh_TW/simulation/covalent-bonds>`_
* `Band Structure <http://phet.colorado.edu/zh_TW/simulation/band-structure>`_

_________________________________________________


WORK EXPERIENCE
--------------------

**2014 - Present**: Senior Engineer, Innovation Digital System, System Software Development Division, Hon Hai Precision IND. CO., LTD. --Responsible for Image recognition algorithms, hand gesture control algorithms, HTML5 acceleration (`WebCL`_), GPGPU applications and development of Android input systems.

**2005 - 2008**: Research assistant in Physics department, National Central University.
--Built and maintained PC clusters and Linux web/mail servers. Built algorithms and models from scratch to simulate chemical and biological materials under statistical mechanics circumstances. [`6`_-\ `8`_]

**2003 - 2005**: Military service

_________________________________________________

SPECIALTIES
--------------------------

* Applied Statistics, Machine Learning, and Mathematical Modeling

 #. Time Series Analysis
 #. Genetic Algorithm
 #. Monte Carlo Method
 #. Optimization Techniques

* Theoretical and Computational Physics

 #. Statistical Physics
 #. Strongly-correlated Systems
 #. Long-time Dynamics
 #. Molecular Dynamics
 #. Molecular Biology
 #. Condensed Matter Physics
 #. Complex Systems

* Reduced Statistical Methods and Diffusion Theory

 #. Mode-coupling Approaches for long-time behaviors
 #. Generalized `Diffusion Equation`_ (GDE)
 #. Optimized `Rouse-Zimm`_ Local Dynamics (ORZLD)

* Parallel Computing Techniques

 #. Open Computing Language (`OpenCL`_)
 #. PC Cluster Computing using Open Message Passing Interface (`OpenMPI`_/`MPICH`_)

* Web-based Technologies

 #. HTML5 and CSS
 #. Data Visualization using JavaScript (`D3.js`_)
 #. `XML`_ (`libxml2`_)

* Computer Vision, Hand Gesture Control, and Image Recognition

 #. Open Source Computer Vision (`OpenCV`_)
 #. Linux/Android Camera and Input Subsystems
 #. `Arduino`_ and Embedded System Programming

* Open Source Projects for science and education

* Statistical Mechanics, Quantum Mechanics, Chemical Physics, and Applied Mathematics

* Software Management and Engineering

 #. `Git`_
 #. Unified Modeling Language (`UML`_)
 #. `CMake`_, `GNU Make`_

* Algorithms and programming language teaching

 #. C++ and C
 #. Python, `NumPy`_, and `Matplotlib`_
 #. Regular Expression
 #. Matlab
 #. GNU Scientific Library (`GSL`_)
 #. Linux System Programming (IPC, thread, socket...)
 #. Linux Shell Script
 #. Fortran
 #. Latex

* System Administrator with experience in Linux

 #. PC Clusters
 #. Web Servers
 #. Mail Servers


_________________________________________________

AWARD
--------

* `Best Team Presentation Award`_, `4th Hope Meeting`_, 2012, Japan.

_________________________________________________

INVITED TALK
--------------
“Open Source in Physics", `International Conference on Open Source 2009`_, Taiwan (`download slides`_)

_________________________________________________


PUBLICATIONS
---------------

(**Download the paper by clicking the title**)

.. _1:

1. `Exploration of hydrogen bond networks and potential energy surfaces of methanol clusters with a two-stage clustering algorithm <http://sophAi.github.io/arch_2013/files_2013/cv/  PJ_Hsu_ref_12.pdf>`_,
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

6. `Comparative study of cluster  Ag17Cu2  by instantaneous normal mode analysis and by isothermal Brownian-type molecular dynamics simulation <http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_ref_07.pdf>`_,
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

OTHER INFORMATION
-----------------

* PhD certificate: `link 1`_ and `link 2`_.

* PhD transcripts: `link`_.

* PhD thesis:

*Molecular dynamics simulations of a fragment of the protein transthyretin and metallic clusters diagnosed by the ultra-fast shape recognition technique, time series segmentation, time series cross correlation analysis and diffusion theory method* (`download thesis`_)

_________________________________________________

RECOMMENDED BY
----------------

* \ `鄭王曜`_\  教授(中央大學物理系，Email: wycheng@ncu.edu.tw /電話:(03)4227151#65337)
* \ `陳永富`_\  教授(中央大學物理系， Email: yfuchen@cc.ncu.edu.tw /電話:(03)4227151#65375)
* \ Dr. `Arnaldo Rapallo`_ (ISMAC, Italy. Email: rapallo@ismac.cnr.it)

_________________________________________________

.. 文章結尾

.. 超連結(URL)目的區

.. _Molecular Science and Technology: http://tigp.iams.sinica.edu.tw/

.. _TIGP: http://tigp.sinica.edu.tw/

.. _National Central University: http://www.phy.ncu.edu.tw/

.. _GestureCV: http://github.com/sophAi/GestureCV

.. _CL-VAF: https://github.com/sophAi/clvaf.git

.. _MPI-Tool: https://github.com/sophAi/mpitool.git

.. _PTMBHGA: https://github.com/sophAi/ptmbhga.git

.. _PTMD: https://github.com/sophAi/ptmd.git

.. _D-Tool: https://github.com/sophAi/dtool.git

.. _TCOM: https://github.com/sophAi/tcom.git

.. _International Conference on Open Source 2009: http://www.slat.org/icos2009/xoops/modules/tinyd0/index.php?id=10

.. _Arnaldo Rapallo: http://www.ismac.cnr.it/pagine/pagina.aspx?ID=Modelling001&L=IT

.. _Siew Ann Cheong: https://www.linkedin.com/pub/siew-ann-cheong/22/384/4b4

.. _San-Kiong Lai: http://www.phy.ncu.edu.tw/english.php?folder=faculty&page=detail.php&pk=7

.. _4th Hope Meeting: http://www.jsps.go.jp/english/e-hope/gaiyou4.html

.. _download slides: http://sophAi.github.io/arch_2013/files_2013/cv/PJ_Hsu_icos2009.pdf

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

.. _Click here to see the D3.js demonstration: http://sophai.github.io/arch_2013/stories/cv.html#data-visualization

.. _Click here to view the demonstration on YouTube: http://sophai.github.io/arch_2013/stories/cv.html#gesturecv

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
