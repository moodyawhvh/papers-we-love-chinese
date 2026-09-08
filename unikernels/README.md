> 🌐 本文档由 [papers-we-love/papers-we-love](https://github.com/papers-we-love/papers-we-love) 翻译,英文原版见原项目。
>
> 注:论文标题保留英文原名以便检索原文,全部链接保持原样;小节标题与说明文字已译为中文。

# Unikernels(单内核)

## 第一波:轻量级内核(微内核,microkernels)

* [HYDRA: the kernel of a multiprocessor operating system](https://kilthub.cmu.edu/articles/HYDRA_--_the_kernel_of_a_multiprocessor_operating_system/6606224/files/12096734.pdf)(HYDRA: 多处理器操作系统的内核)
* [Two years of experience with a μ-Kernel based OS](https://dl.acm.org/citation.cfm?id=122124)(基于 μ 内核的操作系统两年实践)
* [A persistent system in real use-experiences of the first 13 years](https://os.itec.kit.edu/downloads/publ_1993_liedtke_persistent-system-in-real-use.pdf)(实际使用中的持久化系统: 前 13 年的经验)
* [SPIN: An extensible microkernel for application-specific operating system services](https://apps.dtic.mil/dtic/tr/fulltext/u2/a293537.pdf)(SPIN: 面向应用特定操作系统服务的可扩展微内核)
* [Extensibility safety and performance in the SPIN operating system](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.117.6702&rep=rep1&type=pdf)(SPIN 操作系统中的可扩展性、安全性与性能)
* [Policy/mechanism separation in Hydra](http://www.cse.psu.edu/~trj1/cse543-f12/docs/p132-levin-hydra.pdf)(Hydra 中的策略/机制分离)
* [Improving IPC by kernel design](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.55.9939&rep=rep1&type=pdf)(通过内核设计改进 IPC)

## 第二波:云计算优化(exokernel 外核、multikernel 多内核)

* [Exokernel: An operating system architecture for application-level resource management](http://pages.cs.wisc.edu/~remzi/Classes/736/Spring2014/Papers/exo-sosp95.pdf)(Exokernel: 面向应用级资源管理的操作系统架构)
* [Exterminate all operating system abstractions](http://studies.ac.upc.es/doctorat/ENGRAP/hotos-jeremiad.pdf)(消灭所有操作系统抽象)
* [The Clive Operating System](http://github.com/fjballest/docs/blob/master/clivesys.pdf)(Clive 操作系统)
* [The Multikernel: A new OS architecture for scalable multicore systems](http://www.cse.iitd.ac.in/~sbansal/csl862-os/readings/barrelfish.pdf)(Multikernel: 面向可扩展多核系统的新操作系统架构)
* [IX: A Protected Dataplane Operating System for High Throughput and Low Latency](https://www.usenix.org/system/files/conference/osdi14/osdi14-paper-belay.pdf)(IX: 高吞吐低延迟的受保护数据平面操作系统)
* [The IX Operating System: Combining Low Latency, High Throughput, and Efficiency in a Protected Dataplane](https://infoscience.epfl.ch/record/223617/files/tocs16-ix.pdf)(IX 操作系统: 在受保护数据平面中兼得低延迟、高吞吐与高效率)
* [Contiki - a lightweight and flexible operating system for tiny networked sensors](http://dunkels.com/adam/dunkels04contiki.pdf)(Contiki: 面向微型联网传感器的轻量灵活操作系统)
* [Arrakis: The Operating System Is the Control Plane](https://dl.acm.org/citation.cfm?id=2812806)(Arrakis: 操作系统即控制平面)
* [Embracing diversity in the Barrelfish manycore operating system](http://www.barrelfish.org/publications/barrelfish_mmcs08.pdf)(在 Barrelfish 多核操作系统中拥抱硬件多样性)
* [Decoupling Cores, Kernels, and Operating Systems](https://www.usenix.org/system/files/conference/osdi14/osdi14-paper-zellweger.pdf)(解耦处理器核、内核与操作系统)

## Unikernels:基于 libOS 的定制化编译期特化

### 引言(Introduction)

* [Unikernels: Library Operating Systems for the Cloud](http://unikernel.org/files/2013-asplos-mirage.pdf)(Unikernels: 面向云的库操作系统)
* [Unikernels: the rise of the virtual library operating system](https://cacm.acm.org/magazines/2014/1/170866-unikernels/fulltext)(Unikernels: 虚拟库操作系统的崛起)
* [Maximizing hypervisor scalability using minimal virtual machines](https://core.ac.uk/download/pdf/35074556.pdf)(用最小虚拟机最大化 hypervisor 可扩展性)
* [Breaking up is hard to do: security and functionality in a commodity hypervisor](https://open.library.ubc.ca/media/download/pdf/24/1.0052016/1)(拆分之难: 通用 hypervisor 中的安全性与功能性)
* [A case for high performance computing with virtual machines](http://mvapich.cse.ohio-state.edu/static/media/publications/abstract/huangwei-ics06.pdf)(用虚拟机做高性能计算的理由)
* [Comparing the robustness of POSIX operating systems](https://users.ece.cmu.edu/~koopman/ballista/ftcs99/ftcs99.pdf)(POSIX 操作系统的健壮性对比)
* [Exploring the Design Space of Combining Linux with Lightweight Kernels for Extreme Scale Computing](http://www.mcs.anl.gov/events/workshops/ross/2015/slides/ross2015-gerofi.pdf)(探索 Linux 与轻量级内核结合以支撑极限规模计算的设计空间)
* [Using kernel hypervisors to secure applications](https://ieeexplore.ieee.org/abstract/document/646188)(用内核态 hypervisor 保护应用安全)

### 具体的 libOS 实现(Specific libOS implementations)

* [IncludeOS: A minimal, resource efficient unikernel for cloud services](http://oda.oslomet.no/oda-xmlui/bitstream/handle/10642/3189/1321835.pdf)(IncludeOS: 面向云服务的极简、资源高效 unikernel)
* [OSv—optimizing the operating system for virtual machines](https://www.usenix.org/system/files/conference/atc14/atc14-paper-kivity.pdf)(OSv: 为虚拟机优化操作系统)
* [ClickOS and the art of network function virtualization](https://www.usenix.org/system/files/conference/nsdi14/nsdi14-paper-martins.pdf)(ClickOS 与网络功能虚拟化之道)
* [Enabling fast, dynamic network processing with clickos](http://conferences.sigcomm.org/sigcomm/2013/papers/hotsdn/p67.pdf)(用 ClickOS 实现快速动态的网络处理)
* [The rump kernel: A tool for driver development and a toolkit for applications](https://www.netbsd.org/gallery/presentations/justin/2015_AsiaBSDCon/justincormack-abc2015.pdf)(rump kernel: 驱动开发工具与应用工具箱)
* [Flexible operating system internals: the design and implementation of the anykernel and rump kernels](https://aaltodoc.aalto.fi/bitstream/handle/123456789/6318/isbn9789526049175.pdf?sequence=1)(灵活的操作系统内部结构: anykernel 与 rump kernel 的设计与实现)
* [Rump Kernels: No OS? No Problem!](https://www.usenix.org/system/files/login/articles/login_1410_03_kantee.pdf)(Rump Kernels: 没有操作系统?没问题!)
* [HermitCore: A Unikernel for Extreme Scale Computing](https://dl.acm.org/citation.cfm?id=2931093)(HermitCore: 面向极限规模计算的 unikernel)
* [llamaOS: A Solution for Virtualized High-Performance Computing Clusters](https://ieeexplore.ieee.org/document/6969511)(llamaOS: 虚拟化高性能计算集群的一种方案)
* [KylinX: A Dynamic Library Operating System for Simplified and Efficient Cloud Virtualization](https://www.usenix.org/conference/atc18/presentation/zhang-yiming)(KylinX: 简化高效云虚拟化的动态库操作系统)

### 性能、对比与分析(Performance, comparisons and analysis)

* [The impact of operating system structure on memory system performance](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.52.4651&rep=rep1&type=pdf)(操作系统结构对内存系统性能的影响)
* [Hypervisors vs. Lightweight Virtualization: A Performance Comparison](https://www.researchgate.net/profile/Roberto_Morabito/publication/273756984_Hypervisors_vs_Lightweight_Virtualization_A_Performance_Comparison/links/550a83660cf26198a63afb10.pdf)(Hypervisor 与轻量级虚拟化: 性能对比)
* [A performance evaluation of rump kernels as a multi-server os building block on sel4](http://trustworthy.systems/publications/csiro_full_text/Elphinstone_ZMH_17.pdf)(rump kernel 作为 seL4 上多服务器操作系统构建块的性能评估)
* [An updated performance comparison of virtual machines and linux containers](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.471.9242&rep=rep1&type=pdf)(虚拟机与 Linux 容器的最新性能对比)
* [My VM is Lighter (and Safer) than your Container](https://dl.acm.org/citation.cfm?id=3132763)(我的 VM 比你的容器更轻(也更安全))
* [Security of OS-level virtualization technologies: Technical report](https://arxiv.org/pdf/1407.4245v1.pdf)(操作系统级虚拟化技术的安全性: 技术报告)
* [Time Provisioning Evaluation of KVM, Docker and Unikernels in a Cloud Platform](http://repositorio.pucrs.br/dspace/bitstream/10923/14178/2/Time_provisioning_evaluation_of_KVM_Docker_and_Unikernels_in_a_Cloud_Platform.pdf)(云平台中 KVM、Docker 与 Unikernel 的时间供给评估)

### Unikernel 的应用(Applications of Unikernels)

* [Tardigrade: Leveraging Lightweight Virtual Machines to Easily and Efficiently Construct Fault-Tolerant Services](https://www.usenix.org/node/189029)(Tardigrade: 利用轻量级虚拟机轻松高效地构建容错服务)
* [Unikernel-based approach for software-defined security in cloud infrastructures](https://hal.inria.fr/hal-01798793/document)(基于 unikernel 的云基础设施软件定义安全方法)
* [FADES: Fine-Grained Edge Offloading with Unikernels](http://home.in.tum.de/~ding/files/fades-pre-camera.pdf)(FADES: 用 unikernel 实现细粒度边缘卸载)
* [Enterprise IoT security and scalability: how unikernels can improve the status Quo](http://aura.abdn.ac.uk/bitstream/handle/2164/7988/PID4488667.pdf?sequence=1&isAllowed=y)(企业 IoT 的安全与扩展性: unikernel 如何改善现状)
* [Unikernels Everywhere: The Case for Elastic CDNs](https://dl.acm.org/citation.cfm?id=3050757)(Unikernel 无处不在: 弹性 CDN 的理由)
* [Towards minimalistic, virtualized content caches with minicache](http://cnp.neclab.eu/projects/minicache/minicache-workshop.pdf)(用 minicache 迈向极简的虚拟化内容缓存)
* [Jitsu: Just-in-time summoning of unikernels](https://www.usenix.org/system/files/conference/nsdi15/nsdi15-paper-madhavapeddy.pdf)(Jitsu: unikernel 的即时召唤)
* [Enabling fast, dynamic network processing with clickOS](http://conferences.sigcomm.org/sigcomm/2013/papers/hotsdn/p67.pdf)(用 ClickOS 实现快速动态的网络处理)
* [uniprof: A Unikernel Stack Profiler](https://flosch.eu/papers/2017-sigcomm-uniprof.pdf)(uniprof: unikernel 栈分析器)
* [On the Fly TCP Acceleration with Miniproxy](https://arxiv.org/pdf/1605.06285.pdf)(用 Miniproxy 实现即时 TCP 加速)
* [Unikernel monitors: extending minimalism outside of the box](https://www.usenix.org/system/files/conference/hotcloud16/hotcloud16_williams.pdf)(Unikernel 监控器: 将极简主义延伸到"盒子"之外)
* [Unikernels As Processes](https://dl.acm.org/doi/pdf/10.1145/3267809.3267845)(把 unikernel 当作进程来用)
* [On the Fly Orchestration of Unikernels: Tuning and Performance Evaluation of Virtual Infrastructure Managers](https://arxiv.org/pdf/1809.07701.pdf)(unikernel 的即时编排: 虚拟基础设施管理器的调优与性能评估)
* [Live updating in Unikernels](https://www.duo.uio.no/bitstream/handle/10852/59240/45/live-updating-unikernels.pdf)(unikernel 中的热更新)
