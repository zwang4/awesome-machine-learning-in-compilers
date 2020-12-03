# Awesome machine learning for compilers and program optimisation 
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-YES-green.svg)](https://github.com/zwang4/awesome-machine-learning-in-compilers/graphs/commit-activity)

A curated list of awesome research papers, datasets, and tools for applying machine learning techniques to compilers and program optimisation.


## Contents
- [Papers](#papers)
   - [Survey](#survey)
   - [Iterative Compilation and Compiler Option Tuning](#iterative-compilation-and-compiler-option-tuning)
   - [Instruction-level Optimisation](#instruction-level-optimisation)
   - [Parallelism Mapping and Task Scheduling](#parallelism-mapping-and-task-scheduling)
   - [Languages and Compilation](#languages-and-compilation)
   - [Auto-tuning and Design Space Exploration](#auto-tuning-and-design-space-exploration)
   - [Code Size Reduction](#code-size-reduction)
   - [Cost and Performance Models](#cost-and-performance-models)
   - [Domain-specific Optimisation](#domain-specific-optimisation)
   - [Learning Program Representation](#learning-program-representation)
   - [Enabling ML in Compilers](#enabling-ml-in-compilers)
- [Books](#books)
- [Talks and Tutorials](#talks-and-tutorials)
- [Software](#software)
- [Benchmarks and Datasets](#benchmarks-and-datasets)
- [Conferences](#conferences)
- [Journals](#journals)
- [How to Contribute](#how-to-contribute)

## Papers
#### Survey
- <img src="https://img.shields.io/badge/23-pages-green.svg" alt="23-pages" align="top"> [Machine Learning in Compiler Optimisation](https://zwang4.github.io/publications/pieee18.pdf) - Zheng Wang and Michael O'Boyle, Proceedings of the IEEE, 2018
- <img src="https://img.shields.io/badge/43-pages-green.svg" alt="43-pages" align="top"> [A survey on compiler autotuning using machine learning](https://dl.acm.org/doi/abs/10.1145/3197978) - Amir H. Ashouri, William Killian, John Cavazos, Gianluca Palermo, and Cristina Silvano, ACM Computing Surveys (CSUR), 2018
- <img src="https://img.shields.io/badge/43-pages-green.svg" alt="43-pages" align="top"> [A survey of machine learning for big code and naturalness](https://daniel.perez.sh/talks/2018/ml-bigcode-survey.pdf) - Miltiadis Allamanis, Earl T. Barr, Premkumar Devanbu, and Charles Sutton, ACM Computing Surveys (CSUR), 2018

#### Iterative Compilation and Compiler Option Tuning
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Improved basic block reordering](https://arxiv.org/pdf/1809.04676.pdf) - Andy Newell and Sergey Pupyrev. IEEE Transactions on Computers, 2020. 
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [A Collaborative Filtering Approach for the Automatic Tuning of Compiler Optimisations](https://dl.acm.org/doi/abs/10.1145/3372799.3394361) - Stefano Cereda, Gianluca Palermo, Paolo Cremonesi, and Stefano Doni, LCTES 2020. 
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Autophase: Compiler phase-ordering for hls with deep reinforcement learning](https://proceedings.mlsys.org/paper/2020/file/4e732ced3463d06de0ca9a15b6153677-Paper.pdf). Ameer Haj-Ali, Qijing Huang,  William Moses, John Xiang, Ion Stoica, Krste Asanovic, John Wawrzynek. MLSys 2020.
- <img src="https://img.shields.io/badge/21-pages-green.svg" alt="21-pages" align="top"> [Micomp: Mitigating the compiler phase-ordering problem using optimization sub-sequences and machine learning](https://core.ac.uk/download/pdf/93751619.pdf) - Amir H. Ashouri, Andrea Bignoli, Gianluca Palermo, Cristina Silvano, Sameer Kulkarni, and John Cavazos. ACM Transactions on Architecture and Code Optimization (TACO) 2017.
- <img src="https://img.shields.io/badge/26-pages-green.svg" alt="26-pages" align="top"> [Iterative Schedule Optimization for Parallelization in the
Polyhedron Model](https://www.infosun.fim.uni-passau.de/publications/docs/GGS+17.pdf) - Stefan Ganser, Armin Grösslinger, Norbert Siegmund, Sven Apel, and Christian Lengauer. ACM Transactions on Architecture and Code Optimization (TACO), 2017. 
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [Learning to superoptimize programs](https://arxiv.org/abs/1611.01787v3) - Rudy Bunel, Alban Desmaison, M. Pawan Kumar, Philip H.S. Torr, Pushmeet Kohlim. ICLR 2017
- <img src="https://img.shields.io/badge/25-pages-green.svg" alt="25-pages" align="top"> [Continuous learning of compiler heuristics](https://dl.acm.org/doi/abs/10.1145/2400682.2400705) - Michele Tartara and Stefano Crespi Reghizzi. ACM Transactions on Architecture and Code Optimization (TACO), 2013. 
- <img src="https://img.shields.io/badge/16-pages-green.svg" alt="16-pages" align="top"> [Mitigating the compiler optimization phase-ordering problem using machine learning](https://www.eecis.udel.edu/~cavazos/oopsla-2012.pdf) - Sameer Kulkarni and John Cavazos. OOPSLA 2012.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [An evaluation of different modeling techniques for iterative compilation](https://www.eecis.udel.edu/~cavazos/cases-2011.pdf) - Eunjung Park, Sameer Kulkarni, and John Cavazos. CASES 2011.
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Evaluating iterative optimization across 1000 datasets](https://users.elis.ugent.be/~leeckhou/papers/pldi10.pdf) - Yang Chen, Yuanjie Huang, Lieven Eeckhout, Grigori Fursin, Liang Peng, Olivier Temam, and Chengyong Wu. PLDI 2010
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Iterative optimization in the polyhedral model: Part II, multidimensional time](https://www.eecis.udel.edu/~cavazos/pldi-2008.pdf) - Louis-Noël Pouchet, Cédric Bastoul, Albert Cohen, and John Cavazos. PLDI 2008.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Cole: compiler optimization level exploration](https://users.elis.ugent.be/~leeckhou/papers/cgo08.pdf) - Kenneth Hoste and Lieven Eeckhout. CGO 2008.
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [MILEPOST GCC: machine learning based research compiler](http://www.fursin.net/papers/fmtp2008.pdf) - Grigori Fursin, Cupertino Miranda, Olivier Temam, Mircea Namolaru, Elad Yom-Tov, Ayal Zaks, Bilha Mendelson et al., 2008
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Evaluating heuristic optimization phase order search algorithms](http://www.cs.fsu.edu/~whalley/papers/cgo07.pdf) - J. W. Davidson, Gary S. Tyson, D. B. Whalley, and P. A. Kulkarni. CGO 2007. 
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Rapidly selecting good compiler optimizations using performance counters](http://ebonilla.github.io/papers/cavazos-et-al-cgo-2007.pdf) - John Cavazos, Grigori Fursin, Felix Agakov, Edwin Bonilla, Michael FP O'Boyle, and Olivier Temam. CGO 2007. 
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Using machine learning to focus iterative optimization](http://homepages.inf.ed.ac.uk/bfranke/Publications/cgo-2006.pdf) - Felix Agakov, Edwin Bonilla, John Cavazos, Björn Franke, Grigori Fursin, Michael FP O'Boyle, John Thomson, Marc Toussaint, and Christopher KI Williams. CGO 2006. 
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Method-specific dynamic compilation using logistic regression](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.132.4370&rep=rep1&type=pdf) - John Cavazos and Michael FP O'boyle. OOPSLA 2005. 
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [Predicting unroll factors using supervised classification](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.93.2788&rep=rep1&type=pdf) - Mark Stephenson and Saman Amarasinghe. CGO 2005. 
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Fast searches for effective optimization phase sequences](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.93.2788&rep=rep1&type=pdf) - Prasad Kulkarni, Stephen Hines, Jason Hiser, David Whalley, Jack Davidson, and Douglas Jones. PLDI 2004. 


#### Instruction-level Optimisation
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [NeuroVectorizer: end-to-end vectorization with deep reinforcement learning](https://people.eecs.berkeley.edu/~krste/papers/neurovectorizer-cgo2020.pdf) - Ameer Haj-Ali, Nesreen K. Ahmed, Ted Willke, Yakun Sophia Shao, Krste Asanovic, and Ion Stoica. CGO 2020. 
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Unleashing the Power of Learning: An Enhanced Learning-Based Approach for Dynamic Binary Translation](https://www.usenix.org/system/files/atc19-song_0.pdf) - Changheng Song, Wenwen Wang, Pen-Chung Yew, Antonia Zhai, Weihua Zhang. USENIX ATC 2019.
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Compiler Auto-Vectorization with Imitation Learning](https://papers.nips.cc/paper/9604-compiler-auto-vectorization-with-imitation-learning.pdf) - Charith Mendis, Cambridge Yang, Yewen Pu, Saman P. Amarasinghe, Michael Carbin. NeurIPS 2019. 
- <img src="https://img.shields.io/badge/19-pages-green.svg" alt="19-pages" align="top"> [Multi-objective Exploration for Practical Optimization Decisions in Binary Translation](https://dl.acm.org/doi/abs/10.1145/3358185) - Sunghyun Park, Youfeng Wu, Janghaeng Lee, Amir Aupov, and Scott Mahlke. ACM Transactions on Embedded Computing Systems (TECS), 2019. 
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Automatic construction of inlining heuristics using machine learning.](https://dl.acm.org/doi/abs/10.1109/CGO.2013.6495004) - Sameer Kulkarni, John Cavazos, Christian Wimmer, and Douglas Simon. CGO 2013. 
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Automatic tuning of inlining heuristics](http://sc05.supercomputing.org/schedule/pdf/pap274.pdf) - John Cavazos and Michael O'Boyle. SC 2005. 
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Inducing heuristics to decide whether to schedule](https://www.eecis.udel.edu/~cavazos/pldi-2004.pdf) - John Cavazos and J. Eliot B. Moss. PLDI 2003. 
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [Meta optimization: Improving compiler heuristics with machine learning](http://groups.csail.mit.edu/cag/metaopt/papers/metaopt-pldi03.pdf) - Mark Stephenson, Saman Amarasinghe, Martin Martin, and Una-May O'Reilly. PLDI 2003. 
- <img src="https://img.shields.io/badge/7-pages-green.svg" alt="7-pages" align="top"> [Learning to schedule straight-line code](http://papers.nips.cc/paper/1349-learning-to-schedule-straight-line-code.pdf) - J. Eliot B. Moss, Paul E. Utgoff, John Cavazos, Doina Precup, Darko Stefanovic, Carla E. Brodley, and David Scheeff. NeurIPS 1998. 

#### Auto-tuning and Design Space Exploration
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [FBNet: Hardware-Aware Efficient ConvNet Design via Differentiable Neural Architecture Search](https://arxiv.org/pdf/1812.03443.pdf) - Bichen Wu, Xiaoliang Dai, Peizhao Zhang, Yanghan Wang, Fei Sun, Yiming Wu, Yuandong Tian, Peter Vajda, Yangqing Jia, Kurt Keutzer. CVPR 2019.
- <img src="https://img.shields.io/badge/17-pages-green.svg" alt="17-pages" align="top"> [TVM: An automated end-to-end optimizing compiler for deep learning](https://www.usenix.org/system/files/osdi18-chen.pdf) - Tianqi Chen, Thierry Moreau, Ziheng Jiang, Lianmin Zheng, Eddie Yan, Haichen Shen, Meghan Cowan et al., OSDI 2018
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [BOAT: Building auto-tuners with structured Bayesian optimization](https://www.cl.cam.ac.uk/~ey204/teaching/ACS/R244_2018_2019/papers/dalibard_WWW_2017.pdf) - Valentin Dalibard, Michael Schaarschmidt, and Eiko Yoneki, WWW 2017.
- <img src="https://img.shields.io/badge/25-pages-green.svg" alt="25-pages" align="top"> [Cobayn: Compiler autotuning framework using bayesian networks](https://groups.csail.mit.edu/commit/papers/2014/ansel-pact14-opentuner.pdf) - Amir H. Ashouri, Giovanni Mariani, Gianluca Palermo, Eunjung Park, John Cavazos, and Cristina Silvano, ACM Transactions on Architecture and Code Optimization (TACO), 2016. 
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Autotuning algorithmic choice for input sensitivity](http://groups.csail.mit.edu/commit/papers/2015/yding-pldi15-pbinput.pdf) - Yufei Ding, Jason Ansel, Kalyan Veeramachaneni, Xipeng Shen, Una-May O'Reilly, and Saman Amarasinghe. PLDI 2015
- <img src="https://img.shields.io/badge/26-pages-green.svg" alt="26-pages" align="top"> [Fast: A fast stencil autotuning framework based on an optimal-solution space model](http://www.elbagarza.com/pdfs/jia_2015_gpu.pdf) - Yulong Luo, Guangming Tan, Zeyao Mo, and 
Ninghui Sun. ACM Transactions on Architecture and Code Optimization (TACO), 2015. 
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [GPU performance and power tuning using regression trees](https://dl.acm.org/doi/abs/10.1145/2751205.2751214) - Wenhao Jia, Elba Garza, Kelly A. Shaw, and Margaret Martonosi. SC 2015.
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Opentuner: An extensible framework for program autotuning](https://groups.csail.mit.edu/commit/papers/2014/ansel-pact14-opentuner.pdf) - Jason Ansel, Shoaib Kamil, Kalyan Veeramachaneni, Jonathan Ragan-Kelley, Jeffrey Bosboom, Una-May O'Reilly, and Saman Amarasinghe. PACT 2014
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Taming parallel I/O complexity with auto-tuning](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.714.1995&rep=rep1&type=pdf) - Babak Behzad, Huong Vu Thanh Luu, Joseph Huchette, Surendra Byna, Ruth Aydt, Quincey Koziol, and Marc Snir. SC 2013.
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [A multi-objective auto-tuning framework for parallel codes](https://www.researchgate.net/profile/Philipp_Gschwandtner/publication/235436717_A_multi-objective_auto-tuning_framework_for_parallel_codes/links/55b5d86b08aed621de02f1d9/A-multi-objective-auto-tuning-framework-for-parallel-codes.pdf) - Herbert Jordan, Peter Thoman, Juan J. Durillo, Simone Pellegrini, Philipp Gschwandtner, Thomas Fahringer, and Hans Moritsch. SC 2012.
- <img src="https://img.shields.io/badge/8-pages-green.svg" alt="8-pages" align="top"> [Bandit-based optimization on graphs with application to library performance tuning](https://www.icml.cc/Conferences/2009/papers/494.pdf) - Frédéric De Mesmay, Arpad Rimmel, Yevgen Voronenko, and Markus Püschel. ICML 2009.
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Combining models and guided empirical search to optimize for multiple levels of the memory hierarchy](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.532.9511&rep=rep1&type=pdf) - Chun Chen, Jacqueline Chame, and Mary Hall. CGO 2005

#### Parallelism Mapping and Task Scheduling
- <img src="https://img.shields.io/badge/16-pages-green.svg" alt="16-pages" align="top"> [Autopilot: workload autoscaling at Google](https://dl.acm.org/doi/10.1145/3342195.3387524) - Krzysztof Rzadca, Pawel Findeisen, Jacek Swiderski, Przemyslaw Zych, Przemyslaw Broniek, Jarek Kusmierek, Pawel Nowak, Beata Strack, Piotr Witusowski, Steven Hand, John Wilkes. EuroSys 2020. [slides](https://www.eurosys2020.org/wp-content/uploads/2020/04/slides/149_rzadca_slides.pdf)
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Modeling and optimizing NUMA effects and prefetching with machine learning](https://dl.acm.org/doi/10.1145/3392717.3392765) - Isaac Sánchez Barrera, David Black-Schaffer, Marc Casas, Miquel Moretó, Anastasiia Stupnikova, and Mihail Popov. ICS 2020.
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [Poise: Balancing thread-level parallelism and memory system performance in GPUs using machine learning](https://homepages.inf.ed.ac.uk/vnagaraj/papers/hpca19.pdf) - Saumay Dublish, Vijay Nagarajan, and Nigel Tophama. HPCA 2019.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Data and thread placement in NUMA architectures: A statistical learning approach](https://www.mcs.anl.gov/research/projects/argo/publications/2019-icpp-denoyelle.pdf) - Nicolas Denoyelle, Brice Goglin, Emmanuel Jeannot, and Thomas Ropars. ICPP 2019.
- <img src="https://img.shields.io/badge/6-pages-green.svg" alt="6-pages" align="top"> [Code Mapping in Heterogeneous Platforms Using Deep Learning and LLVM-IR](https://iris.polito.it/retrieve/handle/11583/2726074/327896/document_post_print.pdf) - Francesco Barchi, Gianvito Urgese, Enrico Macii, and Andrea Acquaviva. DAC 2019.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Adaptive optimization for OpenCL programs on embedded heterogeneous systems](https://core.ac.uk/download/pdf/83920402.pdf) - Ben Taylor, Vicent Sanz Marco, and Zheng Wang. LCTES 2017.
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [Improving spark application throughput via memory aware task co-location: A mixture of experts approach](https://zwang4.github.io/publications/middleware17.pdf) - Vicent Sanz Marco, Ben Taylor, Barry Porter, and Zheng Wang. Middleware 2017.
- <img src="https://img.shields.io/badge/17-pages-green.svg" alt="17-pages" align="top"> [Quasar: resource-efficient and QoS-aware cluster management](http://csl.stanford.edu/~christos/publications/2014.quasar.asplos.pdf) - Christina Delimitrou, and Christos Kozyrakis. ASPLOS 2014.
- <img src="https://img.shields.io/badge/25-pages-green.svg" alt="25-pages" align="top"> [Automatic and portable mapping of data parallel programs to opencl for gpu-based heterogeneous systems](https://zwang4.github.io/publications/zheng_taco_2015.pdf) - Zheng Wang, Dominik Grewe, and Michael O'boyle. ACM Transactions on Architecture and Code Optimization (TACO), 2014.
- <img src="https://img.shields.io/badge/26-pages-green.svg" alt="26-pages" align="top"> [Integrating Profile-Driven Parallelism Detection and Machine-Learning-Based Mapping](https://zwang4.github.io/publications/taco14.pdf) - Zheng Wang, Georgios Tournavitis, Björn Franke, and Michael FP O'boyle. ACM Transactions on Architecture and Code Optimization (TACO), 2014.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Smart multi-task scheduling for OpenCL programs on CPU/GPU heterogeneous platforms](http://www.lancaster.ac.uk/staff/wangz3/publications/hipc14.pdf) - Yuan Wen, Zheng Wang, and Michael FP O'Boyle. HiPC 2015.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Smart, adaptive mapping of parallelism in the presence of external workload](https://dl.acm.org/doi/abs/10.1109/CGO.2013.6495010) - Murali Krishna Emani, Zheng Wang, and Michael O'Boyle. CGO 2013.
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Partitioning streaming parallelism for multi-cores: a machine learning based approach](https://zwang4.github.io/publications/pact10.pdf) - Zheng Wang and Michael O'Boyle. PACT 2010.
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Qilin: exploiting parallelism on heterogeneous multiprocessors with adaptive mapping](http://www.sphong.net/MICRO_2009.pdf) - Chi-Keung Luk, Sunpyo Hong, and Hyesoon Kim. MICRO 2009.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Mapping parallelism to multi-cores: a machine learning based approach](http://llvm.org/pubs/2009-02-PPoPP-MappingParallelism.pdf) - Zheng Wang and Michael O'Boyle. PPoPP 2009. 


#### Domain-specific Optimisation
- <img src="https://img.shields.io/badge/15-pages-green.svg" alt="15-pages" align="top"> [Bridging the gap between deep learning and sparse matrix format selection](https://people.engr.ncsu.edu/xshen5/Publications/ppopp18.pdf) - Yue Zhao, Jiajia Li, Chunhua Liao and Xipeng Shen. PPoPP 2018. 
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Camel: Smart, Adaptive Energy Optimization for Mobile Web Interactions](http://eprints.whiterose.ac.uk/155720/1/paper.pdf) - Jie Ren, Y. Lu, Petteri Nurmi, Xiaoming Wang, Miao Ma, Ling Gao, Zhanyong Tang, Jie Zheng, and Zheng Wang. INFOCOM 2020. 
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Optimizing sorting with genetic algorithms](http://polaris.cs.uiuc.edu/~garzaran/doc/cgo05.pdf) - Xiaoming Li, Maria Jesus Garzaran, and David Padua. CGO 2005. 


#### Languages and Compilation
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Halide: a language and compiler for optimizing parallelism, locality, and recomputation in image processing pipelines](https://core.ac.uk/download/pdf/20024748.pdf) - Jonathan Ragan-Kelley, Connelly Barnes, Andrew Adams, Sylvain Paris, Frédo Durand, and Saman Amarasinghe, PLDI 2013. 
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [PetaBricks: a language and compiler for algorithmic choice](http://people.csail.mit.edu/cychan/papers/2009pldi-petabricks.pdf) - Jason Ansel, Cy Chan, Yee Lok Wong, Marek Olszewski, Qin Zhao, Alan Edelman, and Saman Amarasinghe. PLDI 2009. 

#### Code Size Reduction
- <img src="https://img.shields.io/badge/7-pages-green.svg" alt="7-pages" align="top"> [Reinforcement Learning Guided Software Debloating](http://www.csl.sri.com/users/gehani/papers/MLSys-2019.DeepOCCAM.pdf) - Nham Le Van, Ashish Gehani, Arie Gurfinkel, Susmit Jha, and Jorge A. Navas. MLSys 2019.
- <img src="https://img.shields.io/badge/9-pages-green.svg" alt="9-pages" align="top"> [Optimizing for reduced code space using genetic algorithms](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.13.1586&rep=rep1&type=pdf) - Keith D. Cooper, Philip J. Schielke, and Devika Subramanian. LCTES 1999. 



#### Cost and Performance Models
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [An Active Learning Method for Empirical Modeling in Performance Tuning](https://ieeexplore.ieee.org/document/9139798) - Jiepeng Zhang, Jingwei Sun, Wenju Zhou, Guangzhong Sun. IPDPS 2020.
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Learning to Optimize Halide with Tree Search and Random Programs](https://dl.acm.org/doi/pdf/10.1145/3306346.3322967) - Andrew Adams, Karima Ma, Luke Anderson, Riyadh Baghdadi, Tzu-Mao Li, Michael Gharbi, Benoit Steiner, Steven Johson, Kayvon Fatahalian, Fredo Durand, Jonathan Ragan-Kelley. ACM Trans Graph, 2019.
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Ithemal: Accurate, portable and fast basic block throughput estimation using deep neural networks](http://proceedings.mlr.press/v97/mendis19a/mendis19a.pdf) - Charith Mendis, Alex Renda, Saman Amarasinghe, and Michael Carbin. ICML 2019.
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Absinthe: Learning an Analytical Performance Model to Fuse and Tile Stencil Codes in One Shot](http://unixer.de/publications/img/gysi-absinthe.pdf) - Tobias Gysi, Tobias Grosser, and Torsten Hoefler. PACT 2019.
- <img src="https://img.shields.io/badge/22-pages-green.svg" alt="22-pages" align="top"> [Predicting new workload or CPU performance by analyzing public datasets](https://yuemmawang.github.io/publications/wang-taco2019.pdf) - Yu Wang, Victor Lee, Gu-Yeon Wei, and David Brooks. ACM Transactions on Architecture and Code Optimization (TACO), 2019.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [Automatic creation of tile size selection models](http://people.rennes.inria.fr/Tomofumi.Yuki/papers/yuki-cgo2010.pdf) - Tomofumi Yuki, Lakshminarayanan Renganarayanan, Sanjay Rajopadhye, Charles Anderson, Alexandre E. Eichenberger, and Kevin O'Brien. CGO 2010. 
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Microarchitecture sensitive empirical models for compiler optimizations](https://www.csa.iisc.ac.in/~srikant/papers-theses/kapil-CGO-2007.pdf) - Kapil Vaswani, Matthew J. Thazhuthaveetil, Y. N. Srikant, and P. J. Joseph. CGO 2007. 
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Accurate static estimators for program optimization](https://dl.acm.org/doi/abs/10.1145/178243.178251) - Tim A. Wagner, Vance Maverick, Susan L. Graham, and Michael A. Harrison. PLDI 1994. 

#### Learning Program Representation
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Deep Program Structure Modeling Through Multi-Relational Graph-based Learning](https://zwang4.github.io/publications/pact20.pdf) - Guixin Ye, Zhanyong Tang, Huanting Wang, Jianbin Fang, Songfang Huang and Zheng Wang. PACT 2020.
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Global Relational Models of Source Code](https://openreview.net/pdf?id=B1lnbRNtwr) - Vincent J. Hellendoorn, Charles Sutton, Rishabh Singh, Petros Maniatis, David Bieber, ICLR 2020. ([Data and Code](https://github.com/VHellendoorn/ICLR20-Great))
- <img src="https://img.shields.io/badge/45-pages-green.svg" alt="45-pages" align="top"> [Learning Semantic Program Embeddings with Graph Interval Neural Network](https://arxiv.org/pdf/2005.09997.pdf) - Yu Wang, Ke Wang, Fengjuan Gao, and Linzhang Wang. OOPSLA 2020.
- <img src="https://img.shields.io/badge/27-pages-green.svg" alt="27-pages" align="top"> [Flow2Vec: Value-Flow-Based Precise Code Embedding](https://yuleisui.github.io/publications/oopsla20.pdf) - Yulei Sui, Xiao Cheng, Guanqin Zhang and Haoyu Wang. OOPSLA 2020.
- <img src="https://img.shields.io/badge/23-pages-green.svg" alt="23-pages" align="top"> [MISIM: An End-to-End Neural Code Similarity System](https://arxiv.org/pdf/2006.05265.pdf) - Fangke Ye, Shengtian Zhou, Anand Venkat, Ryan Marcus, Nesime Tatbul, Jesmin Jahan Tithi, Paul Petersen, Timothy Mattson, Tim Kraska, Pradeep Dubey, Vivek Sarkar and Justin Gottschlich . arXiv 2020.
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [Blended, precise semantic program embeddings](https://dl.acm.org/doi/abs/10.1145/3385412.3385999) - Ke Wang and Zhendong Su. PLDI 2020.
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [LambdaNet: Probabilistic Type Inference using Graph Neural Networks](https://arxiv.org/pdf/2005.02161.pdf) - Jiayi Wei, Maruth Goyal, Greg Durrett, and Isil Dillig. ICLR 2020.
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Compiler-based graph representations for deep learning models of code](https://cfaed.tu-dresden.de/files/Images/people/chair-cc/publications/2002_Brauckmann_CC.pdf) - Alexander Brauckmann, Andrés Goens, Sebastian Ertel, and Jeronimo Castrillon. CC 2020.
- <img src="https://img.shields.io/badge/21-pages-green.svg" alt="24-pages" align="top"> [Generative Code Modeling with Graphs](https://arxiv.org/pdf/1805.08490.pdf) - Marc Brockschmidt, Miltos Allamanis, Alexander L. Gaunt, and Oleksandr Polozov. ICLR 2019.
- <img src="https://img.shields.io/badge/22-pages-green.svg" alt="22-pages" align="top"> [code2seq: Generating sequences from structured representations of code](https://arxiv.org/pdf/1808.01400) - Uri Alon, Shaked Brody, Omer Levy, and Eran Yahav. ICLR 2019.
- <img src="https://img.shields.io/badge/29-pages-green.svg" alt="29-pages" align="top"> [code2vec: Learning distributed representations of code](http://www.cs.technion.ac.il/~mbs/publications/code2vec-popl19.pdf) - Uri Alon, Meital Zilberstein, Omer Levy, and Eran Yahav. POPL 2019.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [COSET: A Benchmark for Evaluating Neural Program Embeddings](https://arxiv.org/pdf/1905.11445.pdf) - Ke Wang, Mihai Christodorescu. arXiv 2019.
- <img src="https://img.shields.io/badge/16-pages-green.svg" alt="16-pages" align="top"> [Learning to Represent Programs with Graphs](https://www.microsoft.com/en-us/research/wp-content/uploads/2017/11/programGraphs.pdf) - Miltiadis Allamanis, Marc Brockschmidt, and Mahmoud Khademi. ICLR 2018.
- <img src="https://img.shields.io/badge/13-pages-green.svg" alt="13-pages" align="top"> [Neural Code Comprehension: A Learnable Representation of Code Semantics](https://papers.nips.cc/paper/7617-neural-code-comprehension-a-learnable-representation-of-code-semantics.pdf) - Tal Ben-Nun, Alice Shoshana Jakobovits, and Torsten Hoefler. NeurIPS 2018.
- <img src="https://img.shields.io/badge/14-pages-green.svg" alt="14-pages" align="top"> [End-to-end deep learning of optimization heuristics](http://homepages.inf.ed.ac.uk/hleather/publications/2017-deepopt-pact.pdf) - Chris Cummins, Pavlos Petoumenos, Zheng Wang, and Hugh Leather ([slides](https://speakerdeck.com/chriscummins/end-to-end-deep-learning-of-optimization-heuristics-pact-17)). PACT 2017.
- <img src="https://img.shields.io/badge/6-pages-green.svg" alt="6-pages" align="top"> [Semantic-aware program sampling](https://www.microsoft.com/en-us/research/wp-content/uploads/2017/11/nips_2017.pdf) - Pratiksha Thaker, Daniel Tarlow, and Marc Brockschmidt. NeurIPS 2017.
- <img src="https://img.shields.io/badge/20-pages-green.svg" alt="20-pages" align="top"> [DeepCoder: Learning to write programs](https://www.microsoft.com/en-us/research/uploads/prod/2017/03/main.pdf) - Matej Balog, Alexander L. Gaunt, Marc Brockschmidt,
Sebastian Nowozin, and Daniel Tarlow. ICLR 2017.
- <img src="https://img.shields.io/badge/7-pages-green.svg" alt="7-pages" align="top"> [Convolutional neural networks over tree structures for programming language processing](http://sei.pku.edu.cn/~zhanglu/Download/AAAI16.pdf) - Lili Mou, Ge Li, Lu Zhang, Tao Wang, and Zhi Jin. AAAI 2016.
- <img src="https://img.shields.io/badge/10-pages-green.svg" alt="10-pages" align="top"> [A Convolutional Attention Network
for Extreme Summarization of Source Code](http://proceedings.mlr.press/v48/allamanis16.pdf) - Miltos Allamanis, Hao Peng, and Charles Sutton. ICML 2016.
- <img src="https://img.shields.io/badge/9-pages-green.svg" alt="9-pages" align="top"> [Structured Generative Models of Natural Source Code](http://proceedings.mlr.press/v32/maddison14.pdf) - Chris Maddison and Daniel Tarlow. ICML 2014.
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Using graph-based program characterization for predictive modeling](https://www.eecis.udel.edu/~cavazos/cgo-2012.pdf) - Eunjung Park, John Cavazos, and Marco A. Alvarez. CGO 2011.
- <img src="https://img.shields.io/badge/11-pages-green.svg" alt="11-pages" align="top"> [Automatic feature generation for machine learning based optimizing compilation](http://homepages.inf.ed.ac.uk/hleather/publications/2009_autofeatures_cgo.pdf) - Hugh Leather, Edwin Bonilla, and Michael O'Boyle. CGO 2009.
   
#### Enabling ML in Compilers
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Synthesizing Benchmarks for Predictive Modeling](https://www.pure.ed.ac.uk/ws/files/29479104/2017_cgo_1.pdf) - Chris Cummins, Pavlos Petoumenos, Zheng Wang, and Hugh Leather ([slides](https://speakerdeck.com/chriscummins/synthesizing-benchmarks-for-predictive-modelling-cgo-17)). CGO 2017.
- <img src="https://img.shields.io/badge/12-pages-green.svg" alt="12-pages" align="top"> [Minimizing the cost of iterative compilation with active learning](http://homepages.inf.ed.ac.uk/hleather/publications/2017-minimitercomp-cgo.pdf) - William Ogilvie, Pavlos Petoumenos, Zheng Wang, and Hugh Leather. CGO 2017.

## Books
- <img src="https://img.shields.io/badge/118-pages-green.svg" alt="118-pages" align="top"> [Automatic Tuning of Compilers Using Machine Learning](https://link.springer.com/book/10.1007/978-3-319-71489-9) - Amir H. Ashouri, Gianluca Palermo, John Cavazos, and Cristina Silvano. Springer 2018.
- <img src="https://img.shields.io/badge/377-pages-green.svg" alt="377-pages" align="top"> [Software Automatic Tuning - From Concepts to State-of-the-Art Results](https://www.springer.com/gp/book/9781441969347) - K Naono, K Teranishi, J Cavazos, and R Suda. Springer 2010.


## Talks and Tutorials
- Saman Amarasinghe, [Compiler 2.0: Using Machine Learning to Modernize Compiler Technology](https://www.youtube.com/watch?v=a1w_NKDVdkI). LCTES 2020.
- Amir Ashouri, [Compiler Autotuning using Machine Learning: A State-of-the-art Review](http://amirashouri.ca/resources/Amir_CompileAutotuning_Talk_2019_Google.pdf). Google Brain 2019.
- Amir Ashouri, [Compiler Autotuning using Machine Learning: A State-of-the-art Review](https://youtu.be/xNixKfDxDZE). Polytechnic University of Milan 2018.

## Software
- [programl](https://github.com/ChrisCummins/ProGraML) - LLVM and XLA IR program representation for machine learning ([paper](https://arxiv.org/pdf/2003.10536.pdf)).
- [NeuroVectorizer](https://github.com/intel/neuro-vectorizer) - Using deep reinforcement learning (RL) to predict optimal vectorization compiler pragmas ([paper](https://arxiv.org/pdf/1909.13639)).
- [TVM](https://tvm.apache.org/) - Open Deep Learning Compiler Stack for cpu, gpu and specialized accelerators ([paper](https://www.usenix.org/system/files/osdi18-chen.pdf); [slides](https://www.usenix.org/sites/default/files/conference/protected-files/osdi18_slides_chen.pdf)).
- [clgen](https://github.com/ChrisCummins/clgen) - Benchmark generator using LSTMs ([paper](https://chriscummins.cc/pub/2017-cgo.pdf); [slides](https://speakerdeck.com/chriscummins/synthesizing-benchmarks-for-predictive-modelling-cgo-17)).
- [COBAYN](https://github.com/amirjamez/COBAYN) - Compiler Autotuning using BNs ([paper](http://amirashouri.ca/resources/COBAYN-ashouri_taco16.pdf)).
- [OpenTuner](https://github.com/jansel/opentuner) - Framework for building domain-specific multi-objective program autotuners ([paper](http://groups.csail.mit.edu/commit/papers/2014/ansel-pact14-opentuner.pdf); [slides](http://groups.csail.mit.edu/commit/papers/2014/ansel-pact14-opentuner-slides.pdf))

## Benchmarks and Datasets
- [BHive](https://github.com/ithemal/bhive) - A Benchmark Suite and Measurement Framework for Validating x86-64 Basic Block Performance Models ([paper](https://groups.csail.mit.edu/commit/papers/19/ithemal-measurement.pdf)).
- [cBench](https://ctuning.org/wiki/index.php/CTools:CBench) - 32 C benchmarks with datasets and driver scripts.
- [PolyBench - Dataset](https://github.com/stefanocereda/polybench_data) - Multiple datasets for Polybench ([paper](https://dl.acm.org/doi/abs/10.1145/3372799.3394361 ))
- [PolyBench](https://github.com/cavazos-lab/PolyBench-ACC) - 31 Stencil and Linear-algebra benchmarks with datasets and driver scripts.
- [PolyBench - Original](http://web.cs.ucla.edu/~pouchet/software/polybench/) - 30 Stencil and Linear-algebra benchmarks with datasets and driver scripts.
- [DeepDataFlow](https://github.com/ChrisCummins/ProGraML/blob/master/programl/Documentation/DataflowDataset.md) - 469k LLVM-IR files and 8.6B data-flow analysis labels for classification ([paper](https://arxiv.org/pdf/2003.10536.pdf)).
- [devmap](https://github.com/ChrisCummins/paper-end2end-dl) - 650 OpenCL benchmark features and CPU/GPU classification labels ([paper](https://chriscummins.cc/pub/2017-pact.pdf); [slides](https://speakerdeck.com/chriscummins/end-to-end-deep-learning-of-optimization-heuristics-pact-17)).

## Conferences
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [ACM SIGPLAN Conference on Programming Language Design and Implementation, PLDI](https://www.sigplan.org/Conferences/PLDI/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [Architectural Support for Programming Languages and Operating Systems, ASPLOS](https://asplos-conference.org/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [ACM SIGPLAN Symposium on Principles and Practice of Parallel Programming, PPoPP](https://dl.acm.org/conference/ppopp)
- <img src="https://img.shields.io/badge/Conference-ACM/IEEE-blue.svg" alt="ACM/IEEE" align="top"> [International Symposium on Code Generation and Optimization, CGO](https://dl.acm.org/conference/cgo)
- <img src="https://img.shields.io/badge/Conference-ACM/IEEE-blue.svg" alt="ACM/IEEE" align="top"> [International Conference on Parallel Architectures and Compilation Techniques, PACT](https://dl.acm.org/conference/cgo)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [Object-oriented Programming, Systems, Languages, and Applications, OOPSLA](http://www.sigplan.org/Conferences/OOPSLA/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Compiler Construction, CC](https://conf.researchr.org/series/CC)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Supercomputing, ICS](http://dblp.uni-trier.de/db/conf/ics/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on High Performance and Embedded Architectures and Compilers, HiPEAC](http://dblp.uni-trier.de/db/conf/hipeac/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Languages, Compilers and Tools for Embedded Systems, LCTES](http://dblp.uni-trier.de/db/conf/lctrts/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Computing Frontiers, CF](http://dblp.uni-trier.de/db/conf/cf)
- <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [International Parallel and Distributed Processing Symposium, IPDPS](http://www.ipdps.org/)
- <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [International Conference for High Performance Computing, Networking, Storage, and Analysis, SC](http://supercomputing.org/)
- <img src="https://img.shields.io/badge/Workshop-Academic-blue.svg" alt="Workshop" align="top"> [Machine Learning and Programming Languages Workshop, MAPL](https://pldi20.sigplan.org/series/mapl)
- <img src="https://img.shields.io/badge/Workshop-Academic-blue.svg" alt="Workshop" align="top"> [Languages and Compilers for Parallel Computing, LCPC](https://dblp.org/db/conf/lcpc/index)
- <img src="https://img.shields.io/badge/Conference-Academic-blue.svg" alt="Academic" align="top"> [International Conference on Learning Representations, ICLR](https://dblp1.uni-trier.de/db/conf/iclr/)
- <img src="https://img.shields.io/badge/Conference-Academic-blue.svg" alt="Academic" align="top"> [Conference on Machine Learning and Systems, MLSys](https://mlsys.org/)
<!---- - <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [EEE/ACM International Symposium on Microarchitecture, Micro](https://dblp1.uni-trier.de/db/conf/micro/)
 - <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [International Conference on Compilers, Architectures, and Synthesis for Embedded Systems, CASES](http://dblp.uni-trier.de/db/conf/cases/index.html) 
 - <img src="https://img.shields.io/badge/Conference-USENIX-blue.svg" alt="USENIX" align="top"> [USENIX Annul Technical Conference, ATC](https://www.usenix.org/conferences/byname/131) 
- <img src="https://img.shields.io/badge/Conference-USENIX-blue.svg" alt="USENIX" align="top"> [USENIX Symposium on Operating Systems Design and Implementation, OSDI](https://dblp.org/db/conf/osdi/index) 
- <img src="https://img.shields.io/badge/Conference-IEEE-blue.svg" alt="IEEE" align="top"> [International Conference on High Performance Computing, Data and Analytics, HiPC](http://dblp.uni-trier.de/db/conf/hipc/index.html) 
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [International Conference on Virtual Execution Environments, VEE](http://dblp.uni-trier.de/db/conf/vee/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [European Conference on Computer Systems, EuroSys](http://dblp.uni-trier.de/db/conf/eurosys/)
- <img src="https://img.shields.io/badge/Conference-ACM-blue.svg" alt="ACM" align="top"> [ACM Symposium on Parallelism in Algorithms and Architectures, SPAA](http://dblp.uni-trier.de/db/conf/spaa/)
- <img src="https://img.shields.io/badge/Conference-IACC-blue.svg" alt="IACC" align="top"> [International Conference on Parallel Processing, ICPP](http://www.wikicfp.com/cfp/program?id=1447&f=International%20Conference%20on%20Parallel%20Processing) 
 - <img src="https://img.shields.io/badge/Conference-ACM/IFIP/USENIX-blue.svg" alt="ACM/IFIP/USENIX" align="top"> [International Middleware Conference, Middleware](http://dblp.uni-trier.de/db/conf/middleware/) 
- <img src="https://img.shields.io/badge/Conference-Academic-blue.svg" alt="ACM" align="top"> [European Conference on Parallel Processing, Euro-Par](http://www.wikicfp.com/cfp/program?id=967&f=European) --->

## Journals
- <img src="https://img.shields.io/badge/Journal-ACM-blue.svg" alt="ACM" align="top"> [ACM Transactions on Architecture and Code Optimization, TACO](https://dl.acm.org/journal/taco)

## How to Contribute

See [Contribution Guidelines](CONTRIBUTING.md). TL;DR: send one of the [maintainers](MAINTAINERS) a [pull request](https://github.com/zwang4/awesome-machine-learning-in-compilers/pulls).
