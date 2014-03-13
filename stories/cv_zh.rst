.. title: Curriculum Vitae (許伯任)
.. slug: cv_zh
.. date: 20140313 14:06:12
.. tags: draft 
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

.. image:: ../../arch_2013/files_2013/cv/gpu_performance.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/gpu_performance.png

**圖(1)** CL-VAF的效能，藍線為CPU效能。 

.. image:: ../../arch_2013/files_2013/cv/clvaf.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/clvaf.png

**圖(2)** 以GPGPU進行向量函數自相關(vector autocorrealtion)的平行化加速計算: (a) 對於一系列向量，(c) 將序列資料依序讀進odd或even buffer; (b) 將自相關函式的kernel編譯並上傳至GPU的work item，並對buffer裡的序列資料進行計算。


CL-VAF [`2`_, `4`_, `5`_, `7`_, `8`_\ ] 是一個以C/C++/OpenCL撰寫的計算程式，透過GPGPU的平行化對隨時間變化的向量進行自相關函數(autocorrelation function)的計算(圖2)，該程式由MPICH版本的\ `TCOM`_\ 修改而來。與Nvidia的CUDA不同在於，OpenCL具有更普遍的相容性，其支援Nvidia、AMD、Intel、Apple甚至是ARM系統，此程式的效能評估是在消費等級的顯示卡上完成的，在更先進的機器上，例如Tesla應該更能發揮其平行化的優勢(圖1)。

`MPI-Tools`_
~~~~~~~~~~~~~~

*MPICH Tools (Shell Script)*

MPI-Tools是一個以Bash Shell Script撰寫的程式，為MPICH快速佈署的工具，可以在極短時間內完成MPICH參數檔、以及CPU分配的環境建立，由於以Shell Script撰寫，幾乎可以在任何Linux/Unix平台上立即執行。


`PTMD`_
~~~~~~~~~~

*Parallel Tempering Molecular Dynamics Simulation Plus Self Analyzers (MPICH/Fortran)*

.. image:: ../../arch_2013/files_2013/cv/ptmd.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/ptmd.png

**圖(3)** PTMD的設計架構。

PTMD [`1`_-\ `5`_\ ]是一個以MPICH/Fortran撰寫的數值計算程式，屬於比較大型的軟體，由敝人於博士學程內獨立完成，該程式以軟體工程的模式進行開發(圖3)，引用版本控制來進行程式的撰寫與維護。PTMD除了能夠利用平行計算進行分子動力學模擬，尚俱備了彈性分析輸出結果的功能，將數值模擬與數值分析視為同等的程式區塊，每個區塊具有標準化的輸入，處理，以及輸出架構，區塊輸出與輸入的資料格式可以互通，最後由一個Parallel Shell主程式進行程式區塊的排程與平行化，將平行化的程式碼獨立出來，除了能快速的將一般數值計算平行化，更能夠依序以模擬1，分析1，模擬2，分析2...等排程來將大量的計算與模擬工作以不間斷的方式進行，例如在一個專題研究裡，我利用這個程式連續半年不間斷地進行10個材料的分子動力學模擬，同時對模擬所得的時間序列資料(例如分子軌跡與能量變化)進行五種以上不同的分析(軌跡分析，自相關時間函數，比熱與統計力學參數計算)，由於Parallel Shell執行上極具彈性，只需將排程腳本編寫完就能讓PTMD一切自動化執行。在多年的平行化程式設計所累積的經驗裡，我了解到除了最佳化程式碼之外，縮短兩個計算工作之間因人工啟動而浪費的閒置時間也是很重要的，利用Parallel Shell縮短閒置時間能夠節省大量的人力與時間，也能夠更方便的擴充數值計算功能。


`PTMBHGA`_
~~~~~~~~~~~~

*Parallel Tempering Multicanonical Basin-hopping Plus Genetic Algorithm (MPICH/Fortran)*

.. image:: ../../arch_2013/files_2013/cv/ptmbhga.png
   :width: 480
   :target: ../../arch_2013/files_2013/cv/ptmbhga.png

**圖(4)** PTMBHGA的設計架構。

PTMBHGA [`1`_-\ `5`_,\ `9`_-\ `11`_\ ] 是另外一個以MPICH/Fortran撰寫的大型最佳化軟體，是我的碩士專題，這個程式結合了基因演算法，平行溫度蒙地卡羅法(Parallel Tempering Monte Carlo)，模擬熱退火(Simulated Annealing)，Multicanonical蒙地卡邏法，還有著名的Basin Hopping法，幾乎網羅文獻中著名的最佳化演算法，其局部最佳化運算子包含Simplex, Conjugate Gradient與LBFG-S演算法，同時也具有平行計算的功能(圖4)。在進行基因演算法的撰寫與學習過程中，我了解到可以將基因演算法的子母世代(generation)視為蒙地卡羅法的取樣步數(sampling step)，而基因運算子(Genetic Operator)可以視為與蒙地卡羅裡的Random Move同等的角色，因此我在基因演算法裡加入蒙地卡羅的機率檢測(Transition Probability)，同時每個子代可以獨立且平行地執行不同溫度參數的蒙地卡羅法，使其可以單獨執行蒙地卡羅，基因演算法，熱退火，平行溫度，甚至是讓這些演算法融合成一種綜合各演算法長處的最佳化方法，經實驗證實其可以準確預測個別最佳化方法獨立執行所無法預測的一些結果，此程式應用性非常廣泛，並已經應用在分子叢集(Cluster)最佳化，最大熵定理計算(Maximal Entropy)，還有石墨烯(Graphene)的結構分析等。透過撰寫這個程式，大大增加了我對最佳化方法的知識與經驗。


`D-Tools`_
~~~~~~~~~~~~~~

*Tools for Diffusion Theory (C/C++)*


D-Tools [`2`_\ ]  是一個以C/C++撰寫的程式，用來輔助Diffusion Theory理論計算的工具程式，這是我的博士論文中，與義大利ISMAC研究單位(相當於台灣的中研院) \ `Arnaldo Rapallo`_\   博士一起進行的生物化學理論研究，在完成PTMD後，我開始學習C/C++與Python，這是當時以C/C++語言完成的軟體之一。


`TCOM`_
~~~~~~~~~

*Vector Autocorrelation Function with MPICH (MPICH/Fortran)*

TCOM [`2`_, `4`_, `5`_, `7`_, `8`_\ ] 是MPICH版本的向量自相關函式計算程式，完成後不久，我以該程式為雛型改寫成OpenCL的版本 (CL-VAF)。


___________________________________________


研究企劃
-----------------------

* **研究主題:** 通用高速平行模擬程式開發

* **研究主旨:** 敝人於求學期間接觸許多國外的大型數值模擬計算專案(例如分子動力學Gromacs與Lammps，第1原理計算VASP, Gaussian, ab initio等)，深深覺得國內類似的數值模擬專案仍是少數，且多分散於各實驗室或研究單位，長期下來因缺乏維護或使用率而產生軟體資源的浪費；吸取國內外大型專案軟體以及自身發展數值模擬軟體的經驗，以通用平行化計算為目標進行數值模擬平台的建立，使其能有效利用GPU，多核心處理器，以及雲端、格點網路計算資源，將平行化的程式碼與數值模擬與分析的程式碼分開處理，以降低程式設計的技術門檻。

初期將針對一般數值計算軟體(例如Matlab)較難發揮的複雜演算法著手，例如最佳化演算法，蒙地卡羅法，基因演算法與分子動力學等，同時包含統計與動態分析功能，使其不但能利用數學模型模擬真實現象，其產生的結果與數據也能同時使用多種方法進行分析與統計，由於分子動力學與最佳化演算法應用層面非常廣泛，涵蓋物理、生物、化學、天文、地球科學、大氣科學、經濟學、藝術、人工智慧辨識、類神經網路、資料庫搜尋，甚至是目前蔚為潮流的巨量資料分析，且彼此之間經常有所交集，這樣的通用模擬架構其實是有迫切與龐大的需求。

* **計劃階段:**

  #. 以Python為膠水語言，作為資料轉換以及平行化(或循序)排程之用途，所轉換的輸入與輸出資料具有統一格式，以C/C++/JAVA/Fortran..等各式語言所寫成的子程式進行讀取並執行計算以得到最佳的效能，同時提供容錯與分析大量資料的能力，程式以開放、跨平台、標準化、高擴充性，同時維持高效能與持續發展為主要的設計方向。
  #. 透過演講與課程教學推廣該軟體，積極尋求大專院校與跨領域研究單位的合作，並協助合作單位進行計算程式的平行化，使其能快速完成程式設計的部份，充份使用高速計算的資源，讓高速計算設備從benchmark測試迅速進入實用階段，同時藉由這樣的合作模式加強與擴充該通用模擬程式的功能。
  #. 建立程式的專頁(SourceForge或github)，採用開放源始碼授權與發佈，成立教學與資源網站，持續降低程式設計的門檻，同時向高中以下的學生進行推廣，以期帶動台灣科學計算的教育普及，並提升國人與下一代的科學水平。

___________________________________________


其他資訊
-----------------------

* 具制訂研究題目、執行研究與分析結果、撰寫並發表成果於國際期刊(SCI)之能力與經驗[`1`_] (獨立作者)。

* 具有豐富的Linux伺服器與PC Cluster建立與管理經驗，在\ `中央大學複雜液體實驗室`_\ 裡從採購、組裝硬體與規劃機房的配線開始，到系統的安裝與設定，從無到有建立了多組實驗室的PC Cluster系統，同時也架設各式伺服器，包含郵件，網頁(實驗室網頁建立)，與版本控制(SVN/Git)伺服器等。

* \ `Best Team Presentation Award`_\ , \ `4th Hope Meeting`_\ , 2012, Japan。

* 2009年開放源碼國際研討會\ `ICOS2009`_\ 物理類開源碼演講者。(\ `slides`_\ )

* \ `教育部EzGo自由軟體專案`_\ PhET線上教育推廣，物理實驗軟體中文翻譯者，翻譯作品如下:


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

* 對於學習充滿熱忱，個性溫和，富團隊合作精神。

.. 文章結尾

.. 超連結(URL)目的區

.. _本網頁pdf版本，請點選下載: http://sophAi.github.io/arch_2013/files_2013/cv/PoJenHsu_Cv.pdf

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

1. `A new perspective of shape recognition to discover the phase transition of finite-size clusters <http://sophAi.github.io/arch_2013/files_2013/cv/JCC_accepted.pdf>`_, 
**P. J. Hsu**, J. Comput. Chem. (2014) (accepted).

.. _2: 

2. `Peptide dynamics by molecular dynamics and diffusion theory methods with improved basis sets <http://sophAi.github.io/arch_2013/files_2013/cv/JCP_accepted.pdf>`_, 
**P. J. Hsu**, S. K. Lai, and A. Rapallo, J. Chem. Phys. (2014) (accepted).

.. _3: 

3. `Precursory Signatures of Protein Folding/Unfolding: From Time Series Correlation Analysis to Atomistic Mechanisms <http://sophAi.github.io/arch_2013/files_2013/cv/JCP_submitted.pdf>`_, 
**P. J. Hsu**, S. A. Cheong, and S. K. Lai. (2014) (submitted).

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

