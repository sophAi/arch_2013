.. title: Curriculum Vitae (許伯任)
.. slug: cv_zh
.. date: 20140301 23:51:42
.. tags: 
.. link: 
.. description: Created at 20130419 13:19:53

.. 請記得加上slug，會以slug名稱產生副檔名為.html的文章
.. 同時，別忘了加上tags喔!

*********************************************
Curriculum Vitae - Po-Jen Hsu / 許伯任
*********************************************

.. 文章起始CONTACT INFORMATION

**Po-Jen Hsu / 許伯任**

Email:   clusterga@gmail.com

Tel:     +886-952-335534

`(本網頁pdf版本，請點選下載) <http://sophAi.github.io/arch_2013/files_2013/cv/PoJenHsu_Cv.pdf>`_

`(English version) <http://sophai.github.io/arch_2013/stories/cv.html>`_

__________________________________________________

教育與經歷
----------

博士班, 中央研究院原子與分子科學研究所國際研究生(TIGP) (2008 - Now)

中央大學物理所專任研究助理 (2005 - 2008)

兵役，海巡下士 (2003 - 2005) 

中央大學物理所碩士 (2000 - 2003)

中央大學物理系學士 (1996 - 2000)

輔仁大學物理系轉學 (1995-1996)

___________________________________________________

程式設計專案
------------

以下程式均為敝人所撰寫，以GNU License (GPL)發佈。(**點選每個子標題可以連結到程式的GitHub專頁**)

`CL-VAF`_
~~~~~~~~~~~

*Vector Autocorrelation Function with GPGPU (OpenCL/C/C++)*

.. image:: ../../arch_2013/files_2013/cv/gpu_performance.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/gpu_performance.png

CL-VAF的效能，藍線為CPU效能。 (**點圖可放大**)

.. image:: ../../arch_2013/files_2013/cv/clvaf.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/clvaf.png

以GPGPU進行向量函數自相關(vector autocorrealtion)的平行化加速計算: (a) 對於一系列向量，(c) 將序列資料依序讀進odd或even buffer; (b) 將自相關函式的kernel編譯並上傳至GPU的work item，並對buffer裡的序列資料進行計算。(**點圖可放大**)


CL-VAF [`1`_, `4`_, `5`_, `7`_, `8`_\ ] 是一個以C/C++/OpenCL撰寫的計算程式，透過GPGPU的平行化對隨時間變化的向量進行自相關函數(autocorrelation function)的計算，該程式由MPICH版本的\ `TCOM`_\ 修改而來。與Nvidia的CUDA不同在於，OpenCL具有更普遍的相容性，其支援Nvidia、AMD、Intel、Apple甚至是ARM系統，此程式的效能評估是在消費等級的顯示卡上完成的，在更先進的機器上，例如Tesla應該更能發揮其平行化的優勢。

`MPI-Tools`_
~~~~~~~~~~~~~~

*MPICH Tools (Shell Script)*

MPI-Tools是一個以Bash Shell Script撰寫的程式，為MPICH快速佈署的工具，可以在極短時間內完成MPICH參數檔、以及CPU分配的環境建立，由於以Shell script撰寫，幾乎可以在任何Linux/Unix平台上立即執行。


`PTMD`_
~~~~~~~~~~

*Parallel Tempering Molecular Dynamics Simulation Plus Self Analyzers (MPICH/Fortran)*

.. image:: ../../arch_2013/files_2013/cv/ptmd.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/ptmd.png

PTMD的設計架構. (**點圖可放大**)

PTMD [`3`_-\ `5`_\ ]是一個以MPICH/Fortran撰寫的數值計算程式，屬於比較大型的軟體(超過10000行程式碼)，由敝人於博士學程內獨立完成，這個程式運用了許多軟體工程的概念，也首度引用版本控制來進行程式的撰寫與維護。PTMD除了能夠利用平行計算進行分子動力學模擬，他還俱備了自我分析結果的能力，這是因為我將數值模擬與數值分析視為同等的程式區塊，每個區塊具有標準化的輸入，處理，以及輸出架構，區塊輸出與輸入的資料格式可以互通，為了達到這個目的，由一個Parallel Shell來進行區塊的排程與平行化，將平行化的程式碼獨立出來，除了能快速的將一般數值計算平行化，更能夠依序以模擬1，分析1，模擬2，分析2...等排程來將大量的計算與模擬工作以不間斷的方式進行，例如在我的博士論文裡，我利用這個程式在半年裡以不間斷的方式進行10個材料的分子動力學模擬，同時對模擬所得的時間序列資料(例如分子軌跡與能量變化)自動進行五種以上不同的分析(軌跡分析，自相關時間函數，比熱與統計力學參數計算)，由於Parallel Shell執行上極具彈性，只要把排程腳本編寫完就能讓PTMD一切自動化去完成。在多年的平行化程式設計所累積的經驗裡，讓我領悟到除了平行與最佳化程式碼之外，善加利用程式執行完到下一個工作開始執行之間CPU閒置的空檔也是很重要的，利用Parallel Shell縮短閒置時間能夠節省大量的人力與時間，也能夠更方便的擴充數值計算功能。


`PTMBHGA`_
~~~~~~~~~~~~

*Parallel Tempering Multicanonical Basin-hopping Plus Genetic Algorithm (MPICH/Fortran)*

.. image:: ../../arch_2013/files_2013/cv/ptmbhga.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/ptmbhga.png

PTMBHGA的設計架構. (**點圖可放大**)

PTMBHGA [`3`_-\ `5`_,\ `9`_-\ `11`_\ ] 是另外一個以MPICH/Fortran撰寫的大型最佳化軟體，是我的碩士專題，這個程式結合了基因演算法，平行溫度蒙地卡羅法(Parallel Tempering Monte Carlo)，模擬熱退火(Simulated Annealing)，Multicanonical蒙地卡邏法，還有著名的Basin Hopping法，幾乎網羅文獻中著名的最佳化演算法，其局部最佳化運算子包含Simplex, Conjugate Gradient跟LBFG-S演算法，同時具有平行計算的能力。在進行基因演算法程式碼的撰寫過程中，我領悟到可以將基因演算法的子母世代(generation)視為蒙地卡羅法的取樣步數(sampling step)，而基因運算子(Genetic Operator)可以視為與蒙地卡羅裡的Random Move同等的角色，因此我在基因演算法裡加入蒙地卡羅的機率檢測(Transition Probability)，同時子代平行化，每個子代可以獨立執行不同溫度參數的蒙地卡羅法，成功的將兩者結合，之後不斷加強程式的功能，例如機率檢測擴充成也可以進行jump walking計算(Multicanonical Monte Carlo)，還有新增更多基因運算子，溫度可以定溫也可以進行熱退火模擬，PTMBHGA後來變成實驗室裡最重要的計算程式，因為他能快速進行高精確度的最佳化計算，還可以分別運行基因演算，蒙地卡羅等演算法，只要透過適當的參數調整即可達到，應用性非常廣泛，除了分子叢集(Cluster)最佳化，近年來還應用在統計的最大熵定理計算(Maximal Entropy)，還有石墨烯(Graphene)的結構分析。透過撰寫這個程式，讓我對最佳化方法有很深入的了解。


`D-Tools`_
~~~~~~~~~~~~~~

*Tools for Diffusion Theory (C/C++)*


D-Tools [`1`_\ ]  是一個以C/C++撰寫的程式，程式碼約為1000多行，是一個用來輔助Diffusion Theory理論計算的工具程式，這是我的博士論文中，與義大利ISMAC研究單位(相當於台灣的中研院) `Arnaldo Rapallo <http://www.ismac.cnr.it/pagine/pagina.aspx?ID=Modelling001&L=IT>`_\  博士一起進行的題目，在完成PTMD後，我將程式設計的重心完全轉移至C/C++與Python，這是當時以C/C++語言完成的作品之一。


`TCOM`_
~~~~~~~~~

*Vector Autocorrelation Function with MPICH (MPICH/Fortran)*

TCOM [`1`_, `4`_, `5`_, `7`_, `8`_\ ] 是MPICH版本的向量自相關函式計算程式，完成後不久，我以該程式為雛型改寫成GPGPU的版本 (CL-VAF)。



___________________________________________

研究企劃
-----------------------

___________________________________________

其他資訊
-----------------------

* 在\ `中央大學複雜液體實驗室 <http://www.phy.ncu.edu.tw/~cplx/index.html>`_\ 裡，我從採購硬體與組裝配件開始，到系統的安裝與測試，幾乎是從0開始打造了實驗室的PC Cluster機房環境，同時也架設了各式伺服器，包含郵件，網頁(實驗室網頁建立)，以及版本控制(SVN/Git)伺服器。

* `Best Team Presentation Award <../../arch_2013/files_2013/cv/hope_award.jpg>`_, `4th Hope Meeting <http://www.jsps.go.jp/english/e-hope/gaiyou4.html>`_, 2012, Japan.

* 2009年 `ICOS2009`_\ 物理類主要演講者. (`slides <../../arch_2013/files_2013/cv/icos2009.pdf>`_)

* 教育部\ `EzGo <http://ossacc.moe.edu.tw/uploads/datafile/ezgo7_linux/_ezgo.html>`_\ 專案的PhET線上教育推廣，物理實驗軟體的中文翻譯者，翻譯作品如下:

  #. `Davission-Germer Experiment <http://phet.colorado.edu/zh_TW/simulation/davisson-germer>`_
  #. `Stern-Gerlach Experiment <http://phet.colorado.edu/zh_TW/simulation/stern-gerlach>`_
  #. `Quantum Wave Interference <http://phet.colorado.edu/zh_TW/simulation/quantum-wave-interference>`_
  #. `Quantum Tunneling <http://phet.colorado.edu/zh_TW/simulation/quantum-tunneling>`_
  #. `Quantum Bound States <http://phet.colorado.edu/zh_TW/simulation/bound-states>`_
  #. `Covalent Bonds <http://phet.colorado.edu/zh_TW/simulation/covalent-bonds>`_
  #. `Band Structure <http://phet.colorado.edu/zh_TW/simulation/band-structure>`_

* 應用統計(Python) [`3`_\ ]，時間序列分析(Time series analysis) [`2`_\ ]，數值模擬(Matlab/Octave)課程教學。

* PC Cluster/GPGPU 計算環境的建立與系統設定，Linux伺服器架設，平行計算程式(MPICH/OpenCL)課程教學。

* 統計物理，量子物理，應用數學，計算機概論，數值模擬，演算法課程教學。

* 自由軟體推廣，科學計算軟體專案建立，大型軟體程式設計，Latex課程教學。


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

發表文獻
------------------

(**點選題目可下載發表期刊文章**)

.. _1:

1. Peptide dynamics by molecular dynamics and diffusion theory methods with improved basis sets,
**P. J. Hsu**, S. K. Lai, and A. Rapallo, J. Chem. Phys. (submitted).

.. _2: 

2. Weak correlation effect on the folding of transthyretin fragment studied by the shape similarity technique and time series methods,
**P. J. Hsu**, S. A. Cheong, and S. K. Lai, Europhys Lett. (accepted).

.. _3: 

3. A new perspective of shape recognition to discover the phase transition of finite-size clusters,
**P. J. Hsu**, J. Comput. Chem. (accepted).

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

