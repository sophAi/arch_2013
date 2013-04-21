.. title: Curriculum Vitae (許伯任)
.. slug: cv
.. date: 2013-04-21 15:15:25
.. tags: 
.. link: 
.. description: Created at 2013-04-19 13:19:53

.. 請記得加上slug，會以slug名稱產生副檔名為.html的文章
.. 同時，別忘了加上tags喔!

*********************************************
Curriculum Vitae - Po-Jen Hsu / 許伯任
*********************************************

.. 文章起始CONTACT INFORMATION

Name: **Po-Jen Hsu / 許伯任**

Email"   clusterga@gmail.com

Tel:     +886-952-335534

__________________________________________________

Ph.D Candidate, TIGP, IAMS, Academia Sinica (2008 - Now)

Research Assistant in Physics, National Central University (2005 - 2008)

Military Service (2003 - 2005) 

M.S. in Physics, National Central University (2000 - 2003)

B.S. in Physics, National Central University (1996 - 2000)

___________________________________________________

PROJECT 
-------

The following softwares were developed by me and can be modified and distributed under GNU License (GPL). **Click on each subtitle will lead you to the corresponding github repositories**. 

`CL-VAF`_
~~~~~~~~~~~

*Vector Autocorrelation Function with GPGPU (OpenCL/C/C++)*

.. image:: ../../arch_2013/files_2013/cv/gpu_performance.png
   :width: 360
   :target: ../../arch_2013/files_2013/cv/gpu_performance.png

Performance of CL-VAF. (click on image to enlarge)

.. image:: ../../arch_2013/files_2013/cv/clvaf.png
   :width: 360
   :target: ../..//arch_2013/files_2013/cv/clvaf.png

Three steps of the vector autocorrelation calculation using GPGPU. For a time series of vectors (a), load data to odd or even buffer sequentially (c). Then, assign the vector autorrelation function for each work item in GPU (b). (click on image to enlarge)

The CL-VAF [`1`_, `2`_, `4`_, `5`_] uses the power of GPGPU to calculate the autocorrelation function of multi-dimensional vectors. The code was modified from my another project **TCOM** with carefully designed GPGPU parallelism. Instead of using CUDA, I chose OpenCL because of the platform transferability. OpenCL is supported by vast manufactures including Nvidia, AMD, Intel, ARM (Mobile devices), Apple, and so on whereas CUDA is only applicable on an Nvidia machine. The benchmark was made based on the consumer-level GPU. For more advanced models such as Nvidia Tesla, the performance should be further improved.

`MPI-Tools`_
~~~~~~~~~~~~~~

*MPICH Tools (Shell Script)*

The MPI-Tools has vast functionalities which allow users to construct and deploy the parallel computing in a minute. It's written in shell script to achieve the highest platform transferability.

`PTMD`_
~~~~~~~~~~

*Parallel Tempering Molecular Dynamics Simulation Plus Self Analyzers (MPICH/Fortran)*

.. image:: ../../arch_2013/files_2013/cv/ptmd.png
   :width: 360
   :target: ../../arch_2013/files_2013/cv/ptmd.png

Framework of PTMD. (click on image to enlarge)

The PTMD [`1`_ - `5`_] is an implementation of the software engineering. It's possible to  run numerical simulations and analyzes the results iteratively and automatically. The parallel computing shell allows most kinds of computation to be set and ran in parallel easily. Up to now, most analyzers were designed for time series clustering, time series statistics, and moment analysis.

`PTMBHGA`_
~~~~~~~~~~~~

*Parallel Tempering Multicanonical Basin-hopping Plus Genetic Algorithm (MPICH/Fortran)*

.. image:: ../../arch_2013/files_2013/cv/ptmbhga.png
   :width: 360
   :target: ../../arch_2013/files_2013/cv/ptmbhga.png

Framework of PTMBHGA. (click on image to enlarge)

The PTMBHGA [`6`_, `7`_, `8`_] is a combination of several state-of-art optimization techniques, including genetic algorithm, parallel tempering Monte Carlo, simulated annealing, basing-hopping, and multicanonical Monte Carlo. The program was designed to be flexible for either a single run  or integration of any optimization technique. I gained most knowledge of optimization from this project.


`D-Tools`_
~~~~~~~~~~~~~~

*Tools for Diffusion Theory (C/C++)*

The D-tools helps reducing the tedious preparation of the diffusion theory calculation. This is one topic of my Ph.D thesis collaborated with Dr. Arnaldo Rapallo. 

`TCOM`_
~~~~~~~~~

*Vector Autocorrelation Function with MPICH (MPICH/Fortran)*

The TCOM [`1`_, `2`_, `4`_, `5`_] is an MPICH version of vector autocorrelation calculation. Later, I wrote CL-VAF with GPGPU implemented.

I also use matlab and python for light-weight computation and figure organization. 

___________________________________________

OTHER INFORMATION
-----------------------

#. Constructor and maintainer of PC clusters (Linux/Unix) and mail/subversion (SVN/Git) system in `Prof. San-Kiong Lai's Lab <http://www.phy.ncu.edu.tw/~cplx/index.html>`_.
#. `Best Team Presentation Award <../../arch_2013/files_2013/cv/hope_award.jpg>`_, `4th Hope Meeting <http://www.jsps.go.jp/english/e-hope/gaiyou4.html>`_, 2012, Japan.
#. Main speaker of Open Source in Physics in `ICOS2009`_. (`slides <../../arch_2013/files_2013/cv/icos2009.pdf>`_)
#. Chinese Translation of Phet Project in Physics.

  a. `Davission-Germer Experiment <http://phet.colorado.edu/zh_TW/simulation/davisson-germer>`_
  #. `Stern-Gerlach Experiment <http://phet.colorado.edu/zh_TW/simulation/stern-gerlach>`_
  #. `Quantum Wave Interference <http://phet.colorado.edu/zh_TW/simulation/quantum-wave-interference>`_
  #. `Quantum Tunneling <http://phet.colorado.edu/zh_TW/simulation/quantum-tunneling>`_
  #. `Quantum Bound States <http://phet.colorado.edu/zh_TW/simulation/bound-states>`_
  #. `Covalent bonds <http://phet.colorado.edu/zh_TW/simulation/covalent-bonds>`_
  #. `Band Structure <http://phet.colorado.edu/zh_TW/simulation/band-structure>`_

#. Open Source and parallel computing lectures.

.. 文章結尾

.. 超連結(URL)目的區

.. _CL-VAF: https://github.com/sophAi/clvaf.git

.. _MPI-Tools: https://github.com/sophAi/mpitool.git

.. _PTMBHGA: https://github.com/sophAi/ptmbhga.git

.. _PTMD: https://github.com/sophAi/ptmd.git

.. _D-Tools: https://github.com/sophAi/dtool.git

.. _TCOM: https://github.com/sophAi/tcom.git

.. _ICOS2009: http://www.slat.org/icos2009/xoops/modules/tinyd0/index.php?id=10




.. 註腳(Footnote)與引用(Citation)區

_________________________________________________

PUBLICATIONS
------------------

(Click on the title to download the paper)

.. 1. **P.J. Hsu**, S.A. Cheong, and S.K. Lai, "Identifying the precursors of protein folding/unfolding using shape recognition and time series methods" (to be submitted)

.. 2. **P.J. Hsu** and S.K. Lai, "Shape recognition and time series analysis in nanoclusters" (to be submitted)

.. 3. **P.J. Hsu**, A. Rapallo, and S.K. Lai, "Hybrid basis sets of diffusion theory in peptide fragments of transthyretin" (in preparation)

.. _1: 

1. P.H. Tang, T.M. Wu, **P.J. Hsu**, and S.K. Lai, J. Chem. Phys. 137, 244304 (2012), "`Melting behavior of Ag14 cluster: An order parameter by instantaneous normal modes <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/84.pdf>`_"

.. _2:

2. P.H. Tang, T.M. Wu, T.W. Yen, S.K. Lai, and **P.J. Hsu**, J. Chem. Phys. 135, 094302 (2011), “`Comparative study of cluster Ag17Cu2 by instantaneous normal mode analysis and by isothermal Brownian-type molecular dynamics simulation <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/82.pdf>`_"

.. _3:

3. S.K. Lai, Y.T. Lin, **P.J. Hsu**, and S.A. Cheong, Compt. Phys. Commun. 182, 1013 (2011), “`Dynamical study of metallic clusters using the statistical method of time series clustering <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/81.pdf>`_"

.. _4:

4. T.W. Yen, **P.J. Hsu**, and S.K. Lai, e-J. Surf. Sci. Nanotech. 7, 149-156 (2009), “`Melting behavior of noble-metal-based bimetallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/78.pdf>`_"

.. _5:

5. **P.J. Hsu**, J.S. Luo, S.K. Lai, J.F. Wax, and J-L Bretonnet, J. Chem. Phys. 129, 194302 (2008), “`Melting scenario in metallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/77.pdf>`_"

.. _6:

6. **P.J. Hsu** and S.K. Lai, J. Chem. Phys. 124, 044711 (2006), “`Structure of bimetallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/71.pdf>`_"

.. _7:

7. L. Zhan, B. Piwowar, W.K. Liu, **P.J. Hsu**, S.K. Lai, and Jeff Z. Y. Chen, J. Chem. Phys. 120, 5536 (2004), “`Multi-canonical basin-hopping: a new global optimization method for complex systems <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/63.pdf>`_"

.. _8:

8. S.K. Lai, **P.J. Hsu**, K.L. Wu, W.K. Liu, and M. Iwamatsu, J. Chem. Phys. 117, 10715 (2002), “`Structures of metallic clusters: mono- and polyvalent metals <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/61.pdf>`_"


