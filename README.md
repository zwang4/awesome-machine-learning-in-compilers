# Awesome machine learning for compilers and program optimisation
This repository contains a curated list of awesome research papers, datasets and tools for applying machine learning techniques to compilers and program optimisation. 


## Contents
- [Conferences](#conferences)
- [Papers](#papers)
   - [Survey](#survey)
   - [Choosing Compiler Flags](#choosing-compiler-flags)
   - [Cost Models](#cost-models)
   - [Parallelism Mapping](#parallelism-mapping)
   - [Auto-tuning](#auto-tuning)
   - [Learning Program Representation](#learning-program-representation)
   - [Tackling ML Hurdles in Compilers](#tackle-ml-hurdles-in-compilers)
- [Tutorials](#tutorials)
- [Software](#software)
- [Datasets](#datasets)
- [Contributions](#contributions)

## Conferences
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [ACM SIGPLAN Conference on Programming Language Design and Implementation, PLDI](https://www.sigplan.org/Conferences/PLDI/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [Architectural Support for Programming Languages and Operating Systems, ASPLOS](https://asplos-conference.org/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [ACM SIGPLAN Symposium on Principles and Practice of Parallel Programming, PPoPP](https://dl.acm.org/conference/ppopp)
- <img src="https://img.shields.io/badge/Conference-ACM/IEEE-blue.svg" alt="ACM/IEEE" align="top"> [International Symposium on Code Generation and Optimization, CGO](https://dl.acm.org/conference/cgo)
- <img src="https://img.shields.io/badge/Conference-ACM/IEEE-blue.svg" alt="ACM/IEEE" align="top"> [International Conference on Parallel Architectures and Compilation Techniques, PACT](https://dl.acm.org/conference/cgo)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [Object-oriented Programming, Systems, Languages, and Applications, OOPSLA](http://www.sigplan.org/Conferences/OOPSLA/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Compiler Construction, CC](https://conf.researchr.org/series/CC)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [European Conference on Computer Systems, EuroSys](http://dblp.uni-trier.de/db/conf/eurosys/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Supercomputing, ICS](http://dblp.uni-trier.de/db/conf/ics/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [ACM Symposium on Parallelism in Algorithms and Architectures, SPAA](http://dblp.uni-trier.de/db/conf/spaa/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on High Performance and Embedded Architectures and Compilers, HiPEAC](http://dblp.uni-trier.de/db/conf/hipeac/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Virtual Execution Environments, VEE](http://dblp.uni-trier.de/db/conf/vee/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Languages, Compilers and Tools for Embedded Systems, LCTES](http://dblp.uni-trier.de/db/conf/lctrts/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Computing Frontiers, CF](http://dblp.uni-trier.de/db/conf/cf)
- <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [International Parallel and Distributed Processing Symposium, IPDPS](http://www.ipdps.org/)
- <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [International Conference for High Performance Computing, Networking, Storage, and Analysis, SC](http://supercomputing.org/)
- <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [International Conference on Compilers, Architectures, and Synthesis for Embedded Systems, CASES](http://dblp.uni-trier.de/db/conf/cases/index.html)
- <img src="https://img.shields.io/badge/Conference-USENIX-blue.svg" alt="USENIX" align="top"> [USENIX Annul Technical Conference, ATC](https://www.usenix.org/conferences/byname/131)
- <img src="https://img.shields.io/badge/Conference-USENIX-blue.svg" alt="USENIX" align="top"> [USENIX Symposium on Operating Systems Design and Implementation, OSDI](https://dblp.org/db/conf/osdi/index)
- <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [International Conference on High Performance Computing, Data and Analytics, HiPC](http://dblp.uni-trier.de/db/conf/hipc/index.html)
- <img src="https://img.shields.io/badge/Conference-IACC-blue.svg" alt="IACC" align="top"> [International Conference on Parallel Processing, ICPP](http://www.wikicfp.com/cfp/program?id=1447&f=International%20Conference%20on%20Parallel%20Processing)
- <img src="https://img.shields.io/badge/Conference-ACM/IFIP/USENIX-blue.svg" alt="ACM/IFIP/USENIX" align="top"> [International Middleware Conference, Middleware](http://dblp.uni-trier.de/db/conf/middleware/)
- <img src="https://img.shields.io/badge/Conference-Academic-blue.svg" alt="ACM" align="top"> [European Conference on Parallel Processing, Euro-Par](http://www.wikicfp.com/cfp/program?id=967&f=European)
- <img src="https://img.shields.io/badge/Workshop-Academic-blue.svg" alt="Workshop" align="top"> [Machine Learning and Programming Languages Workshop, MAPL](https://pldi20.sigplan.org/series/mapl)
- <img src="https://img.shields.io/badge/Workshop-Academic-blue.svg" alt="Workshop" align="top"> [Languages and Compilers for Parallel Computing, LCPC](https://dblp.org/db/conf/lcpc/index)
- <img src="https://img.shields.io/badge/Conference-Academic-blue.svg" alt="Academic" align="top"> [International Conference on Learning Representations, ICLR](https://dblp1.uni-trier.de/db/conf/iclr/)
- <img src="https://img.shields.io/badge/Conference-Academic-blue.svg" alt="Academic" align="top"> [Conference on Machine Learning and Systems, MLSys](https://mlsys.org/)

## Papers
#### Survey
- <img src="https://img.shields.io/badge/23-pages-green.svg" alt="23-pages" align="top"> [Machine Learning in Compiler Optimisation](https://zwang4.github.io/publications/pieee18.pdf) - Zheng Wang and Michael O'Boyle, Proceedings of the IEEE, 2018
- <img src="https://img.shields.io/badge/43-pages-green.svg" alt="43-pages" align="top"> [A survey on compiler autotuning using machine learning](https://dl.acm.org/doi/abs/10.1145/3197978) - Ashouri, Amir H., William Killian, John Cavazos, Gianluca Palermo, and Cristina Silvano, ACM Computing Surveys (CSUR), 2018
- <img src="https://img.shields.io/badge/43-pages-green.svg" alt="43-pages" align="top"> [A survey of machine learning for big code and naturalness](https://daniel.perez.sh/talks/2018/ml-bigcode-survey.pdf) - Allamanis, Miltiadis, Earl T. Barr, Premkumar Devanbu, and Charles Sutton, ACM Computing Surveys (CSUR), 2018

#### Choosing Compiler Flags
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [A Collaborative Filtering Approach for the Automatic Tuning of Compiler Optimisations](https://dl.acm.org/doi/abs/10.1145/3372799.3394361) - Cereda, Stefano, Gianluca Palermo, Paolo Cremonesi, and Stefano Doni, LCTES 2020. 
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Autophase: Compiler phase-ordering for hls with deep reinforcement learning](https://ieeexplore.ieee.org/abstract/document/8735549). Qijing Huang, Ameer Haj-Ali, William Moses, John Xiang, Ion Stoica, Krste Asanovic, John Wawrzynek. FCCM 2019.
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [MILEPOST GCC: machine learning based research compiler](http://www.fursin.net/papers/fmtp2008.pdf) - Grigori Fursin, Cupertino Miranda, Olivier Temam, Mircea Namolaru, Elad Yom-Tov, Ayal Zaks, Bilha Mendelson et al., 2008
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Using machine learning to focus iterative optimization](http://homepages.inf.ed.ac.uk/bfranke/Publications/cgo-2006.pdf) - Agakov, Felix, Edwin Bonilla, John Cavazos, Björn Franke, Grigori Fursin, Michael FP O'Boyle, John Thomson, Marc Toussaint, and Christopher KI Williams, CGO 2006. 

#### Auto-tuning
- <img src="https://img.shields.io/badge/17-pages-green.svg" alt="17-pages" align="top"> [TVM: An automated end-to-end optimizing compiler for deep learning](https://www.usenix.org/system/files/osdi18-chen.pdf) - Tianqi Chen, Thierry Moreau, Ziheng Jiang, Lianmin Zheng, Eddie Yan, Haichen Shen, Meghan Cowan et al., OSDI 2018
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Opentuner: An extensible framework for program autotuning](https://groups.csail.mit.edu/commit/papers/2014/ansel-pact14-opentuner.pdf) - Jason Ansel, Shoaib Kamil, Kalyan Veeramachaneni, Jonathan Ragan-Kelley, Jeffrey Bosboom, Una-May O'Reilly, and Saman Amarasinghe, PACT 2014


#### Parallelism Mapping
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Partitioning streaming parallelism for multi-cores: a machine learning based approach](https://zwang4.github.io/publications/pact10.pdf) - Zheng Wang and Michael O'Boyle, PACT 2010.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Mapping parallelism to multi-cores: a machine learning based approach](http://llvm.org/pubs/2009-02-PPoPP-MappingParallelism.pdf) - Zheng Wang and Michael O'Boyle, PPoPP 2009. 

#### Cost Models
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Learning to Optimize Halide with Tree Search and Random Programs](https://dl.acm.org/doi/pdf/10.1145/3306346.3322967) - Andrew Adams, Karima Ma, Luke Anderson, Riyadh Baghdadi, Tzu-Mao Li, Michael Gharbi, Benoit Steiner, Steven Johson, Kayvon Fatahalian, Fredo Durand, Jonathan Ragan-Kelley. ACM Trans Graph, 38(4), 2019.


#### Learning Program Representation
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Compiler-based graph representations for deep learning models of code](https://cfaed.tu-dresden.de/files/Images/people/chair-cc/publications/2002_Brauckmann_CC.pdf) - Alexander Brauckmann, Andrés Goens, Sebastian Ertel, and Jeronimo Castrillon, CC 2020.
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [End-to-end deep learning of optimization heuristics](http://homepages.inf.ed.ac.uk/hleather/publications/2017-deepopt-pact.pdf) - Chris Cummins, Pavlos Petoumenos, Zheng Wang, and Hugh Leather, PACT 2017.
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Automatic feature generation for machine learning based optimizing compilation](http://homepages.inf.ed.ac.uk/hleather/publications/2009_autofeatures_cgo.pdf) - Hugh Leather, Edwin Bonilla, and Michael O'Boyle. CGO 2009.

#### Tackling ML Hurdles in Compilers

## Tutorials

## Software
- [programl](https://github.com/ChrisCummins/ProGraML) - LLVM and XLA IR program representation for machine learning.
- [clgen](https://github.com/ChrisCummins/clgen) - Benchmark generator using LSTMs ([paper](https://chriscummins.cc/pub/2017-cgo.pdf)).
- [TVM](https://tvm.apache.org/) - Open Deep Learning Compiler Stack for cpu, gpu and specialized accelerators ([paper](https://www.usenix.org/system/files/osdi18-chen.pdf); [slides](https://www.usenix.org/sites/default/files/conference/protected-files/osdi18_slides_chen.pdf))
- [OpenTuner](https://github.com/jansel/opentuner) - Framework for building domain-specific multi-objective program autotuners ([paper](http://groups.csail.mit.edu/commit/papers/2014/ansel-pact14-opentuner.pdf); [slides](http://groups.csail.mit.edu/commit/papers/2014/ansel-pact14-opentuner-slides.pdf))

## Datasets
- [cBench](https://ctuning.org/wiki/index.php/CTools:CBench) - 32 C benchmarks with datasets and driver scripts.
- [DeepDataFlow](https://github.com/ChrisCummins/ProGraML/blob/master/programl/Documentation/DataflowDataset.md) - 469k LLVM-IR files and 8.6B data-flow analysis labels for classification labels.
- [devmap](https://github.com/ChrisCummins/paper-end2end-dl) - 650 OpenCL benchmark features and CPU/GPU classification labels.

## Contributions

See [Contributions.md](Contributions.md). TL;DR: send me ([@zwang4](https://github.com/zwang4)) a [pull request](https://github.com/zwang4/awesome-machine-learning-in-compilers/pulls).
