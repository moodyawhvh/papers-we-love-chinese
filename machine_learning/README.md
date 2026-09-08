> 🌐 本文档由 [papers-we-love/papers-we-love](https://github.com/papers-we-love/papers-we-love) 翻译,英文原版见原项目。
>
> 注:论文标题保留英文原名以便检索原文,全部链接保持原样;说明文字已译为中文。

# 机器学习(Machine Learning)


## 外部论文(External Papers)

* [Top 10 algorithms in data mining](https://www.researchgate.net/publication/29467751_Top_10_algorithms_in_data_mining)(数据挖掘十大算法)

  虽然"十大"很难评,但这篇论文收录了 10 个非常重要的数据挖掘/机器学习算法。

* [A Few Useful Things to Know about Machine Learning](http://homes.cs.washington.edu/~pedrod/papers/cacm12.pdf)(关于机器学习,你应该知道的几件实用事)

  正如标题所言,文中包含许多机器学习的实用技巧与易踩的坑。
* [Random Forests](https://www.stat.berkeley.edu/~breiman/randomforest2001.pdf)(随机森林)

  随机森林的开山之作。
* [Conditional Random Fields: Probabilistic Models for Segmenting and Labeling Sequence Data](http://repository.upenn.edu/cgi/viewcontent.cgi?article=1162&context=cis_papers)(条件随机场: 序列数据切分与标注的概率模型)

  提出条件随机场(CRF)作为构建概率模型的框架的论文。
* [Support-Vector Networks](http://rd.springer.com/content/pdf/10.1007%2FBF00994018.pdf)(支持向量网络)

  用于分类的支持向量网络(SVM)的最初论文。

* [The Fast Johnson-Lindenstrauss Transforms](https://www.cs.princeton.edu/~chazelle/pubs/FJLT-sicomp09.pdf)(快速 Johnson-Lindenstrauss 变换)

    Johnson-Lindenstrauss 变换(JLT)指出:存在一个尺寸为 `k x d` 的矩阵,其中 `k = O(1/eps^2 log d)`,从这个分布中抽取的矩阵 A 有很高概率能在 epsilon 误差内保持成对距离(例如 `(1-eps) * ||x-y|| < ||Ax - Ay|| < (1+eps) ||x-y||`)。这篇论文首次证明 JLT 可以用少于 `O(kd)` 次运算完成(也就是说,不必做完整的矩阵乘法)。作者用这个更快的算法构造出了已知最快的近似最近邻算法之一。

    *Ailon, Nir, and Bernard Chazelle. "The fast Johnson-Lindenstrauss transform and approximate nearest neighbors." SIAM Journal on Computing 39.1 (2009): 302-322. Available: https://www.cs.princeton.edu/~chazelle/pubs/FJLT-sicomp09.pdf*

* [Applications of Machine Learning to Location Data](http://www.berkkapicioglu.com/wp-content/uploads/2013/11/thesis_final.pdf)(机器学习在位置数据上的应用)

  利用机器学习设计并分析借助位置数据的新颖算法。

* ["Why Should I Trust You?" Explaining the Predictions of Any Classifier](http://www.kdd.org/kdd2016/papers/files/rfp0573-ribeiroA.pdf)("我为什么该信你?": 解释任意分类器的预测,即 LIME)

  这篇论文提出了一种以可解释方式解释任意分类器预测结果的技术。

* [Multiple Narrative Disentanglement: Unraveling *Inﬁnite Jest*](http://aclanthology.org/N12-1001.pdf)(多叙事分离: 解开《无尽玩笑》)

  使用无监督自然语言处理方法,对 David Foster Wallace 那部 1000 页小说中的叙事者进行分类。

* [ImageNet Classification with Deep Convolutional Neural Networks](http://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)(用深度卷积神经网络做 ImageNet 分类)

  这篇论文提出了 AlexNet——一种大幅超越当时最先进图像分类算法的神经网络架构,被广泛视为深度学习的突破性时刻。

* [Interpretable machine learning: definitions, methods, and applications](https://arxiv.org/pdf/1901.04592.pdf)(可解释机器学习: 定义、方法与应用)

  这篇论文介绍了可解释机器学习这一快速兴起领域的基础。

* [Distilling the Knowledge in a Neural Network](https://arxiv.org/pdf/1503.02531.pdf)(蒸馏神经网络中的知识)

  这篇开创性论文提出了一种把神经网络集成(ensemble)中的知识蒸馏到单个模型里的方法。

* [Truncation of Wavelet Matrices: Edge Effects and the Reduction of Topological Control](https://reader.elsevier.com/reader/sd/pii/0024379594000395?token=EB0AA78D59A9648480596F018EFB72E0A02FD5FA70326B24B9D501E1A6869FE72CC4D97FA9ACC8BAB56060D6C908EC83)(小波矩阵的截断: 边缘效应与拓扑控制的约化),作者 Freedman

  Michael Hartley Freedman 在这篇论文中,借助小波将 Robion Kirby 的"环面技巧"(torus trick)应用于压缩问题。


## 托管论文(Hosted Papers)

* :scroll: **[A Sparse Johnson-Lindenstrauss Transform](dimensionality_reduction/a-sparse-johnson-lindenstrauss-transform.pdf)**(稀疏 Johnson-Lindenstrauss 变换)

    对许多应用而言,JLT 的计算开销仍然很高,一个目标就是尽量减少上述矩阵乘法所需的总运算量。这篇论文证明了 `O(k log d)`(即 `(log(d))^2)` 量级的算法可能可以实现,方法是证明非常稀疏的结构化随机矩阵同样能提供成对距离的 *JL* 保证。

    *Dasgupta, Anirban, Ravi Kumar, and Tamás Sarlós. "A sparse johnson: Lindenstrauss transform." Proceedings of the forty-second ACM symposium on Theory of computing. ACM, 2010. Available: [arXiv/cs/1004:4240](http://arxiv.org/abs/1004.4240)*

* :scroll: **[Towards a unified theory of sparse dimensionality reduction in Euclidean space](dimensionality_reduction/toward-a-unified-theory-of-sparse-dimensionality-reduction-in-euclidean-space.pdf)**(迈向欧氏空间稀疏降维的统一理论)

    这篇论文尝试(从凸分析与泛函分析的角度)为稀疏降维搭建通用的数学框架。第一作者是菲尔兹奖得主,热衷于把巴拿赫空间的技术应用到这个问题上。这是一篇非常技术性的论文,试图回答这样一个问题:"稀疏嵌入什么时候能确定性地存在?"(也就是说,不依赖随机矩阵的抽取。)

    *Bourgain, Jean, and Jelani Nelson. "Toward a unified theory of sparse dimensionality reduction in euclidean space." arXiv preprint arXiv:1311.2542; Accepted in an AMS Journal but unpublished at the moment  (2013). Available: http://arxiv.org/abs/1311.2542*


* :scroll: **[Understanding Deep Convolutional Networks](Understanding-Deep-Convolutional-Networks.pdf)**(理解深度卷积网络),作者 Mallat

  Stéphane Mallat 提出一个模型,通过重整化(renormalisation)来识别深度网络中的自相似结构。[这段 Curt MacMullen 讲重整化的视频](https://www.youtube.com/watch?v=_qjPFF5Gv1I)可以帮助你补充背景。

* :scroll: **[General self-similarity: an overview](General-self-similarity--an-overview.pdf)**(广义自相似: 综述),作者 Leinster

  Leinner 博士的这篇论文以简洁直白的方式描绘了自相似性及其在重整化中的作用。
