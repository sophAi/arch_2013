.. title: Curriculum Vitae (許伯任)
.. slug: cv_zh_Hsu
.. date: 20140313 14:24:34
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

(\ `本網頁pdf版本，請點選下載`_\ )

.. `(English version) <http://sophai.github.io/arch_2013/stories/cv.html>`_

__________________________________________________

教育與經歷
----------

博士班, 中央研究院原子與分子科學研究所國際研究生(TIGP) (2008 - Now)

中央大學物理所專任研究助理 (2005 - 2008)

兵役，海巡 (2003 - 2005) 

中央大學物理所碩士 (2000 - 2003)

中央大學物理系學士 (1996 - 2000)

輔仁大學物理系轉學 (1995-1996)

___________________________________________________

程式設計專案
------------

以下程式均為敝人所獨立撰寫，以GNU License (GPL)發佈。(**點選每個子標題可以連結到程式的GitHub專頁**)

`CL-VAF`_
~~~~~~~~~~~

*Vector Autocorrelation Function with GPGPU (OpenCL/C/C++)*

.. .. image:: ../../arch_2013/files_2013/cv/gpu_performance.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/gpu_performance.png

.. **圖(1)** CL-VAF的效能，藍線為CPU效能。 

.. .. image:: ../../arch_2013/files_2013/cv/clvaf.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/clvaf.png

.. **圖(2)** 以GPGPU進行向量函數自相關(vector autocorrealtion)的平行化加速計算: (a) 對於一系列向量，(c) 將序列資料依序讀進odd或even buffer; (b) 將自相關函式的kernel編譯並上傳至GPU的work item，並對buffer裡的序列資料進行計算。


CL-VAF [`2`_, `4`_, `5`_, `7`_, `8`_\ ] 是一個以C/C++/OpenCL撰寫的計算程式，透過GPGPU的平行化對隨時間變化的向量進行「自相關函數(autocorrelation function)」的計算。

`MPI-Tools`_
~~~~~~~~~~~~~~

*MPICH Tools (Shell Script)*

MPI-Tools是一個以Bash Shell Script撰寫的程式，為MPICH環境的建立與快速佈署之多功能工具，可以在極短時間內生成MPICH的相關參數檔以及將執行程式分配給特定的CPU或PC cluster。以Shell語言為基礎，可以在任何Linux/Unix平台上立即執行。


`PTMD`_
~~~~~~~~~~

*Parallel Tempering Molecular Dynamics Simulation Plus Self Analyzers (MPICH/Fortran)*

.. .. image:: ../../arch_2013/files_2013/cv/ptmd.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/ptmd.png

.. **圖(3)** PTMD的設計架構。

PTMD [`1`_-\ `5`_\ ]是一個以MPICH/Fortran撰寫的數值模擬程式，屬於比較大型的軟體。此程式除了能夠利用平行計算進行分子動力學模擬，尚俱備了彈性分析輸出結果的功能(包含各式時序動態資料與統計資料之分析)。能夠依序以模擬1、分析模擬1之結果、模擬2、分析模擬2之結果...等排程來大幅縮短數值計算因等待人工啟動而閒置的時間，也能讓任何模擬與分析工作自動平行化。


`PTMBHGA`_
~~~~~~~~~~~~

*Parallel Tempering Multicanonical Basin-hopping Plus Genetic Algorithm (MPICH/Fortran)*

.. .. image:: ../../arch_2013/files_2013/cv/ptmbhga.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/ptmbhga.png

.. **圖(4)** PTMBHGA的設計架構。

PTMBHGA [`1`_-\ `5`_,\ `9`_-\ `11`_\ ] 是一個以MPICH/Fortran撰寫的平行化最佳化軟體。該程式包含了基因演算法、平行溫度蒙地卡羅法(Parallel Tempering Monte Carlo)、模擬熱退火(Simulated Annealing)、Multicanonical蒙地卡邏法、Basin Hopping法等各式廣為採用的最佳化演算法，並將這些方法結合成一個綜合各演算法長處的最佳化方法，經實驗證實可以準確預測個別最佳化方法獨立執行所無法預測的一些結果，例如合金分子叢集的最穩定結構[`9`_\ ]，此程式具廣泛的適用性，並已經應用在分子叢集(Cluster)最佳化、最大熵定理計算(Maximal Entropy)及石墨烯(Graphene)的結構分析等。


`D-Tools`_
~~~~~~~~~~~~~~

*Tools for Diffusion Theory (C/C++)*


D-Tools [`2`_\ ]  是一個以C/C++撰寫的程式，用來輔助Diffusion Theory理論計算的工具程式。此為我的博士論文中，與義大利ISMAC研究單位(相當於台灣的中研院) \ `Arnaldo Rapallo`_\   博士一起進行的生物化學理論研究所撰寫的工具軟體。


`TCOM`_
~~~~~~~~~

*Vector Autocorrelation Function with MPICH (MPICH/Fortran)*

TCOM [`2`_, `4`_, `5`_, `7`_, `8`_\ ] 是MPICH版本的平行化向量自相關函式計算程式，為OpenCL版本的CL-VAF之前身。


___________________________________________



其他資訊
-----------------------

* 具制訂研究題目、執行研究與分析結果、撰寫並發表成果於國際期刊(SCI)之能力與經驗[`1`_] 。

* 具有豐富的Linux伺服器與PC Cluster建立與管理經驗。在\ `中央大學複雜液體實驗室`_\ 裡擔任研究助理的期間，敝人從採購機器、組裝硬體，到機房的配置、系統的安裝與設定等，從無到有建立了多組實驗室的PC Cluster系統，同時也架設各式伺服器，包含郵件，網頁(實驗室網頁建立)，與版本控制(SVN/Git)伺服器等。

* \ `Best Team Presentation Award`_\ , \ `4th Hope Meeting`_\ , 2012, Japan。

* 2009年開放源碼國際研討會\ `ICOS2009`_\ 物理類開源碼演講者。(\ `slides`_\ )

* \ `教育部EzGo自由軟體專案`_\ PhET線上教育推廣--物理教學軟體中文翻譯者。翻譯作品如下:


  #. `Davission-Germer Experiment <http://phet.colorado.edu/zh_TW/simulation/davisson-germer>`_
  #. `Stern-Gerlach Experiment <http://phet.colorado.edu/zh_TW/simulation/stern-gerlach>`_
  #. `Quantum Wave Interference <http://phet.colorado.edu/zh_TW/simulation/quantum-wave-interference>`_
  #. `Quantum Tunneling <http://phet.colorado.edu/zh_TW/simulation/quantum-tunneling>`_
  #. `Quantum Bound States <http://phet.colorado.edu/zh_TW/simulation/bound-states>`_
  #. `Covalent Bonds <http://phet.colorado.edu/zh_TW/simulation/covalent-bonds>`_
  #. `Band Structure <http://phet.colorado.edu/zh_TW/simulation/band-structure>`_

* 應用統計(Python) [`3`_\ ]、時間序列分析(Time series analysis) [`2`_\ ]與數值模擬(Matlab/Octave)課程教學。

* PC Cluster/GPGPU 計算環境的建立與系統設定、Linux伺服器架設與管理教學與平行計算程式(MPICH/OpenCL)課程教學。

* 統計物理、量子物理、應用數學、計算機概論、數值模擬與演算法課程教學。

* 自由軟體推廣，科學計算軟體專案建立，大型軟體程式設計，Latex文件撰寫與簡報課程教學。

* 對於學習充滿熱忱，個性溫和，樂於助人，認真負責，富團隊合作精神。

.. 文章結尾

.. 超連結(URL)目的區

.. _本網頁pdf版本，請點選下載: http://sophAi.github.io/arch_2013/files_2013/cv/cv_zh_Hsu.pdf

.. _CL-VAF: https://github.com/sophAi/clvaf.git

.. _MPI-Tools: https://github.com/sophAi/mpitool.git

.. _PTMBHGA: https://github.com/sophAi/ptmbhga.git

.. _PTMD: https://github.com/sophAi/ptmd.git

.. _D-Tools: https://github.com/sophAi/dtool.git

.. _TCOM: https://github.com/sophAi/tcom.git

.. _ICOS2009: http://www.slat.org/icos2009/xoops/modules/tinyd0/index.php?id=10

.. _Arnaldo Rapallo: http://www.ismac.cnr.it/pagine/pagina.aspx?ID=Modelling001&L=IT

.. _中央大學複雜液體實驗室: http://www.phy.ncu.edu.tw/~cplx/index.html

.. _4th Hope Meeting: http://www.jsps.go.jp/english/e-hope/gaiyou4.html

.. _slides: http://sophAi.github.io/arch_2013/files_2013/cv/icos2009.pdf

.. _教育部EzGo自由軟體專案: http://ossacc.moe.edu.tw/uploads/datafile/ezgo7_linux/

.. _Best Team Presentation Award: http://sophAi.github.io/arch_2013/files_2013/cv/hope_award.jpg

.. 註腳(Footnote)與引用(Citation)區

_________________________________________________

發表文獻
------------------

(**點選題目可下載發表期刊文章**)

.. _1:

1. `A new perspective of shape recognition to discover the phase transition of finite-size clusters <http://sophAi.github.io/arch_2013/files_2013/cv/JCC_accepted.pdf>`_, **P. J. Hsu**, J. Comput. Chem. (2014) (accepted).

.. _2: 

2. `Peptide dynamics by molecular dynamics and diffusion theory methods with improved basis sets <http://sophAi.github.io/arch_2013/files_2013/cv/JCP_accepted.pdf>`_, **P. J. Hsu**, S. K. Lai, and A. Rapallo, J. Chem. Phys. (2014) (accepted).

.. _3: 

3. `Precursory Signatures of Protein Folding/Unfolding: From Time Series Correlation Analysis to Atomistic Mechanisms <http://sophAi.github.io/arch_2013/files_2013/cv/JCP_submitted.pdf>`_, **P. J. Hsu**, S. A. Cheong, and S. K. Lai. (2014) (submitted).

.. _4: 

4. `Melting behavior of Ag14 cluster: An order parameter by instantaneous normal modes <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/84.pdf>`_, P. H. Tang, T. M. Wu, **P. J. Hsu**, and S. K. Lai, J. Chem. Phys. 137, 244304 (2012).

.. _5:

5. `Comparative study of cluster Ag17Cu2 by instantaneous normal mode analysis and by isothermal Brownian-type molecular dynamics simulation <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/82.pdf>`_, P. H. Tang, T. M. Wu, T. W. Yen, S. K. Lai, and **P. J. Hsu**, J. Chem. Phys. 135, 094302 (2011).

.. _6:

6. `Dynamical study of metallic clusters using the statistical method of time series clustering <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/81.pdf>`_, S. K. Lai, Y. T. Lin, **P. J. Hsu**, and S. A. Cheong, Compt. Phys. Commun. 182, 1013 (2011).

.. _7:

7. `Melting behavior of noble-metal-based bimetallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/78.pdf>`_, T. W. Yen, **P. J. Hsu**, and S. K. Lai, e-J. Surf. Sci. Nanotech. 7, 149-156 (2009).

.. _8:

8. `Melting scenario in metallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/77.pdf>`_, **P. J. Hsu**, J. S. Luo, S. K. Lai, J. F. Wax, and J-L Bretonnet, J. Chem. Phys. 129, 194302 (2008).

.. _9:

9. `Structure of bimetallic clusters <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/71.pdf>`_, **P. J. Hsu** and S. K. Lai, J. Chem. Phys. 124, 044711 (2006).

.. _10:

10. `Multi-canonical basin-hopping: a new global optimization method for complex systems <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/63.pdf>`_, L. Zhan, B. Piwowar, W. K. Liu, **P. J. Hsu**, S. K. Lai, and Jeff Z. Y. Chen, J. Chem. Phys. 120, 5536 (2004).

.. _11:

11. `Structures of metallic clusters: mono- and polyvalent metals <http://www.phy.ncu.edu.tw/~cplx/main_paper_pdf/61.pdf>`_, S. K. Lai, **P. J. Hsu**, K. L. Wu, W. K. Liu, and M. Iwamatsu, J. Chem. Phys. 117, 10715 (2002).

