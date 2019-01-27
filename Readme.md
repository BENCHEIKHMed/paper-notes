<h1 align="center"> Directory </h1>

### Pantheon: the training ground for Internet congestion-control research

* Author: Francis Y. Yan†, (Stanford University)
* Index: Best Paper at USENIX ATC 2018
* Reading date : 27/01/2019
* Keywords : Congestion Control

The author present the [Pantheon](https://pantheon.stanford.edu), a system taht addresses this by serving as a community " training ground " for research on Internet Protocols and congestion control. There is a common set of benchmark algorithms and a shared evaluation platform, and a public archive of results.
Pantheon can also be used to develop new CC schemes , two of which already published on NSDI 2018. I think this is mysterious and interesting that's why i choose this paper to read.

---

### ECN or Delay: Lessons Learnt from Analysis of DCQCN and TIMELY

* Author: Yibo Zhu (Microsoft;ByteDance)
* Index: CoNEXT 2016 
* Reading date : 20/01/2019
* Keywords : Datacenter transport, RDMA, ECN, delay-based, congestion control

This is also for `[RDMA Section]` paper 2. Aiming at reviewing the classical paper in relative to RDMA. Based on the paper name, we already know that this paper is about the compare of `DCQCN` and `TIMELY`. 

According to the YiboZhu, which is the author of the `DCQCN`: DC networks especially drop-free RoCEv2 networks require efficient cc protocols. `DCQCN(ECN-based)` and `TIMELY(delay-based)` are two recent proposals for this purpose. In this paper, we analyze DCQCN and TIMELY using fluid models and simulations, for stability, convergence, fairness and flow completion time. We uncover several surprising behaviors of these protocols. 

The author also address the broader question: are there fundamental reasons to `prefer either ECN or delay` for end-to-end congestion control in DC Networks ?

* [:heart_decoration: Read More](
)

---

### TIMELY: RTT-based Congestion Control for the DataCenter 

* Author: Radhika Mittal (UC Berkeley)
* Index: SIGCOMM 2015 
* Reading date : 20/01/2019
* Keywords : Datacenter transport, delay-based CC, OS-bypass, RDMA

This is for `[RDMA Section]` paper 2. Aiming at reviewing the classical paper in relative to RDMA. 

Datacenter transports aim to deliver low latency messageing together with high throughput. We show that simple packet delay, measured as `round-trip times` at hosts, is an effective congestion signal without the need for switch feedback. 

- First, we show that advances in NIC hardware have made RTT measurement possible with microsecond accuracy, and that these RTTs are sufficient to estimate switch queueing. 
- Then we describe how TIMELY can adjust transmission rates using RTT gradients to keep packet latency low while delivering high bandwidth. 

TIMELY is the first delay-based CC protocol in datacenter. And it achieves its result despite having an order of magnitude fewer RTT signals.

* [:heart_decoration: Read More](
)

---

### Learning Network by Reproducing Network Result 🦄
* Author: Lisa Yan (Stanford University)
* Index: SIGCOMM 2017 
* Reading date : 19/01/2019
* Keywords : Reproducible research, Teaching computer networks
* Score: 📒📕📘📗

This paper is finished by my Academic Idol Lisa Yan. This paper is so important because [Hope](http://web.stanford.edu/class/cs244/index.html) is a waking [dream](https://reproducingnetworkresearch.wordpress.com/page/2/)．

    I'd like to deal with this course as a student.
    I'd like to do the final pj of this course.

Lisa Yan said that:
> "In the past five years, the graduate networking course at Stanford has assigned over 200 students the task of reproducing results from over 40 networking papers. We began the project as a means of teaching both engineering rigor and critical thinking, qualities that are necessary for careers in networking research and industry. We have observed that reproducing research can simultaneously be a tool for education and a means for students to contribute to the networking community. "

* [:heart_decoration: Read More](https://miqianmimi.github.io/2019/01/20/Reproducing-Network/)

---

### Improving TCP Congestion Control with Machine Intelligence
* Author: Yiming Kong (Georgia Tech)
* Index: SIGCOMM 2018 Workshop
* Reading date: 16/01/2019
* Keywords : Network-> Transport protocols Computing methodologies→ Supervised learning; Reinforcement learning; Machine Learning; Security and Privacy.

This paper is about both off-line and on-line TCP-CC scheme.The writer use both supervised learning and reinforcement learning to train two TCP CC schemes.She use NS2 simulation to prepare for the dumbbell topology network and She set the environment to the basic under-buffered bottleneck network.
Why i choose this paper to read in detail is because it goes into details about the TCP-CC-ML scheme And that helps me to playback the experiment in the paper.

* [:heart_decoration: Read More](https://miqianmimi.github.io/2019/01/19/TCP-CC-ML/)

---

### Stream-based ML for Network Security and Anomaly Detection
* Author: Pavol Mulinka (CTU Czech)
* Index: SIGCOMM 2018 Workshop
* Reading date : 15/01/2019
* Keywords : Machine Learning; Computing methodologies; Security and Privacy.

This paper is about `Data Stream Machine Learning` for `network security and anomaly detection`. And especially for `on-line` questions (in this field the general approach is still off-line learning problem). The experiment result shows that the `adaptive random forests and stochastic gradient descent` models are able to keep up with important `concept drifts` by keeping high accuracy. 

They also introduced Big-DAMA, a big data analytics framework for large scale network traffic monitoring and analysis. 

* [:heart_decoration: Read More](https://miqianmimi.github.io/2019/01/16/Stream-based-ML/)

---

### DCQCN -- Congestion Control for Large-Scale RDMA Deployments
* Author: Yibo Zhu (Microsoft;ByteDance)
* Index: SIGCOMM 2015
* Reading date : 02/01/2019-10/01/2019
* Keywords : Datacenter transport; RDMA; PFC; ECN; Congestion Control 

This is for `[RDMA Section]` paper 1. Aiming at reviewing the classical paper in relative to RDMA. so i choose it due to its high reference in the filed of Datacenter transport. 

This paper in one word, proposing a new way of congestion control to solve the head-of-line blocking and unfairness problem introduced by PFC. This way is very suitable for the RDMA Datacenter and works well with RoCEv2. 

* [:heart_decoration: Read More](https://miqianmimi.github.io/2019/01/11/DCQCN/)

---

### Congestion Control Something to say
* Blog Conclusion of Congestion Control
* Reading date : 7/12/2018
* Keywords : Congestion Control ; Reinforcement Learning

I find a NYC coder's Blog in which it introduced several important concept in Congestion Control. Also with several useful code. So I read his 4 blogs and conclude his words. These 4 blogs are the introduction of CC, the Cubic , the RED , the Reinforcement Learning .

* [:heart_decoration: Read More](https://miqianmimi.github.io/2018/12/07/CC-BLOG/)

---

### Exising TCP CC Algorithm
* Summary of Congestion Control
* Reading date : 5/12/2018
* Keywords : TCP ; Congestion Control 

TCP Congestion Control aims at choose a strategy to find the appropriate cwnd and to acheive the best utility of bandwidth. In this summary, we briefly introduce several different mechanism in TCP CC Algorithm starting from TCP Vegas , TCP Reno , Cubic, BBR and Remy.

* [:heart_decoration: Read More](https://miqianmimi.github.io/2018/12/06/TCP-CC/)

---

### Friends, not Foes - Synthesizing Existing Trnasport Strategies for Data Center Networks
* Author: Ali Munir (Michigan State University)
* Index: SIGCOMM 2014
* Reading date : 3/12/2018
* Keywords : Datacenter transport; Congestion Control 

Many Data Center transports have been proposed in recent times. Contrary to the common perception that they are competitors. We claim that the underlying strategies used in these protocols are , in fact complementary.

So we design `PASE` a transport framework that synthesize existing transport strategies, namely, self-adjusting endpoints (used in TCP style protocols), in-network prioritization (used in pFabric), and arbitration(used in PDQ). PASE is deployment friendly It does not require any changes to the network fabric. Its performance is better than state-of-the-art protocols (pFabric). Using NS2 simulation and testbed experiments.

* [:heart_decoration: Read More](https://miqianmimi.github.io/2018/12/03/PASE/)

---


