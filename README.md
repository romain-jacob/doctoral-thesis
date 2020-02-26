## Leveraging Synchronous Transmissions for the Design of Real-time Wireless Cyber-Physical Systems

Romain Jacob

#### Doctoral Dissertation
This repository contains all source files and visualization notebooks of my doctoral dissertation.  
The [compiled PDF](https://github.com/romain-jacob/doctoral-thesis/raw/master/00_thesis.pdf) is readily available.  
The files are stored on Zenodo for long-term archiving.  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3510184.svg)](https://doi.org/10.5281/zenodo.3510184)

#### Doctoral Examination Presentation
This dissertation was defended successfully on December 17th, 2019 at ETH Zurich, Switzerland.  
The presentation is available under various formats.
- [PDF](https://osf.io/rgkdx/)
- [Source (.pptx)](https://osf.io/6vd9j/)
- [Video (20min)](https://youtu.be/t-cynMz2s0c)

#### How to Cite
> Romain Jacob. 
_Leveraging Synchronous Transmissions for the Design of Real-time Wireless Cyber-Physical Systems_. 
Doctoral Thesis, ETH Zurich, 2020. http://doi.org/10.3929/ethz-b-000401717

or using BibTeX
```TeX
@phdthesis{jacob2020Leveraging,
  title = {Leveraging Synchronous Transmissions for the Design of Real-time Wireless Cyber-Physical Systems},
  author = {Jacob, Romain},
  year = {2020},
  DOI = {10.3929/ethz-b-000401717},
  school = {ETH Zurich},
  language = {en},
  copyright = {Creative Commons Attribution 4.0 International},
  type = {Doctoral Thesis},
  abstract = {Cyber-Physical Systems (CPS) refer to systems where some intelligence isembedded into devices that interact with their environment; that is, collectinginformation from the physical space, processing that information, and takingactions that affect the environment. Automatically turning the heating onwhen room temperature gets cold is one of the simplest example of CPS.Things get more complex when applications are distributed between low-powerdevices that should operate autonomously for multiple years. Then, performingreliable and energy efficient wireless communication becomes paramount.Moreover, applications often specify deadlines; that is, maximal tolerable delaysbetween the execution of distributed tasks. Systems that guarantee to meetsuch deadlines are called real-time systems. Wireless CPS capable of providingreal-time guarantees while using low-power communication technology aredesirable but they are particularly challenging to design. In the past few years, atechnique known as synchronous transmissions (ST) has been shown to enablereliable and energy efficient communication in low-power multi-hop networks.In a nutshell, ST consists in letting multiple devices transmit a packet during thesame time interval; communication is likely to be successful if the transmissionsare well synchronized, hence the name of synchronous transmissions. ST canbe leveraged to realize any multi-hop broadcast – a one-to-all communication –in a given time; a very interesting property for designing real-time systems.While the potential of ST is recognized by the low-power wireless academiccommunity, this technique has not yet been leveraged for the design of CPS.We identify at least three issues that limit the adoption of ST in this domain:(i) ST is difficult to use due to stringent time synchronization requirements:in the order of μs. There is a lack of tools to facilitate the implementationof ST by CPS engineers, which are often not wireless communication experts.(ii) There are only few examples showcasing the use of ST for CPS applicationsand academic works based on ST tend to focus on communication ratherthan applications. Convincing proof-of-concept CPS applications are missing.(iii) The inherent variability of the wireless environment makes performanceevaluation challenging. The lack of an agreed-upon methodology hindersexperiment reproduciblility and limits the confidence in the performance claims.Consequently, we developed support tools and methods to facilitate theevaluation of wireless protocols and the implementation of CPS based on ST.Furthermore, we leveraged ST to design two CPS solutions targeting differentclasses of real-time applications. This dissertation presents these contributions.In Chapter 2, we propose to design and analyze performance evaluationexperiments for networking protocols using a concrete, rational, and statisticallysound methodology. We implement this methodology in a framework calledTriScale which allows to make performance claims with quantifiable levelsof confidence. Furthermore, we leverage the TriScale framework to proposethe first formalized definition of reproducibility for networking experiments.Chapter 3 presents Baloo, a flexible design framework for network stacksbased on ST. Users implement their protocol through the programminginterface offered by Baloo while the framework handles the complex low-level operations; e.g., meeting the time synchronization requirements of ST.We show that Baloo is flexible enough to implement a wide variety of commu-nication protocols while introducing only limited memory and energy overhead.Finally, we design and implement two wireless CPS based on ST:– the Distributed Real-time Protocol (DRP) uses contracts to maximize theflexibility of execution between distributed tasks (Chapter 4);– Time-Triggered Wireless (TTW ) statically co-schedules all task executionsand packet transfers to minimize end-to-end latency (Chapter 5).We demonstrate that real-time guarantees can be provided in a reliable andenergy efficient manner. Furthermore, TTW supports update rates of tens ofms, which is sufficient to perform distributed closed-loop control of invertedpendulums – a fundamental benchmark for control and robotic applications.With this dissertation, we showcase that ST is suitable to meet the requirementsof real-time wireless CPS. Furthermore, we facilitate the implementation ofsuch systems with Baloo, a design framework that makes ST accessible tothe non-expert. Finally, TriScale provides an important building block toconfidently evaluate the performance of networking protocols – an essentialbuilding block of wireless CPS. Building on TriScale, it would be useful to definebenchmark problems representative of different classes of applications to serveas baseline for the evaluation of future wireless CPS solutions. Ultimately, wemust transition from proof-of-concepts to real-world wireless CPS applications;this would be further facilitated by porting Baloo to newer and morepowerful platforms, thereby pushing the limits of achievable performance levels.},
}
```
