> 🌐 本文档由 [papers-we-love/papers-we-love](https://github.com/papers-we-love/papers-we-love) 翻译,英文原版见原项目。
>
> 注:论文标题保留英文原名以便检索原文,全部链接保持原样;说明文字已译为中文。

## 信息检索(Information Retrieval)

信息检索,指的是从一组信息资源中获取与某种信息需求相关的资源的活动。(维基百科如是说。)

收录的文档有:

* [:scroll:](graph_of_word_and_tw_idf.pdf) [Graph of Word and TW-IDF](http://www.lix.polytechnique.fr/~rousseau/papers/rousseau-cikm2013.pdf)(词图与 TW-IDF)- Francois Rousseau & Michalis Vazirgiannis

  传统的信息检索系统在索引中存储词项级的统计信息(通常是词项在每篇文档中出现的频次,即 TF)。这类模型忽略了词项之间的依赖关系,把一篇文档中的词项视为彼此独立出现(因此得名"词袋模型",bag-of-words,名副其实)。在这篇论文中,作者使用一种基于文档图表示的统计量来编码词项间的依赖关系,用基于所构图的新 TW 统计量替换 TF 统计量,取得了显著优于现有流行模型的结果。该论文获得 CIKM 2013 优秀论文提名(honorable mention)。

* [:scroll:](the-pagerank-citation-ranking-bringing-order-to-the-web.pdf) [The PageRank Citation Ranking: Bringing Order to the Web](http://ilpubs.stanford.edu:8090/422/1/1999-66.pdf)(PageRank 引用排名: 给 Web 带来秩序)- Lawrence Page、Sergey Brin、Rajeev Motwani 与 Terry Winograd

  这篇论文提出了 PageRank 算法——当今 Google 搜索引擎的骨架。PageRank 通过评估指向和离开某个网页的超链接数量,并依据页面的链接结构对网页进行排名。作者还在 backrub 系统(也就是后来的 Google 搜索引擎)上实现了 PageRank,详见《[Anatomy of a Large-Scale Hypertextual Web Search Engine](http://infolab.stanford.edu/~backrub/google.html)》,它为整个万维网上的每个网页都计算了 PageRank 值。Google 如今是全球商业上最成功的通用搜索引擎。

* [:scroll:](okapi-at-trec3.pdf) [Okapi at TREC3](http://trec.nist.gov/pubs/trec3/papers/city.ps.gz)(Okapi 在 TREC3)- Stephen E. Robertson、Steve Walker、Susan Jones、Micheline Hancock-Beaulieu 与 Mike Gatford

  这篇论文提出了如今大名鼎鼎的 Okapi 信息检索框架,为排序检索引入了 BM25 排序函数。它是文献中概率检索框架最早的实现之一。BM25 是一个词袋检索函数,其 IDF(逆文档频率)项可以从信息论角度解读:如果查询 q 出现在 n(q) 篇文档中,随机抽取一篇文档且它包含该词项的概率为 p(q) = n(q) / D,其中 D 是文档总数。基于香农噪声信道模型,信息量为 -log(p(q)) = log(D / n(q))。对分子分母同时加常数做平滑,就得到了 BM25 中使用的 IDF 项。BM25 已被证明是最好的概率加权方案之一。由于原文是 PostScript 格式,提交者已按照 Papers We Love 的规范用 ps2pdf 将其转换为 pdf。

* [:scroll:](authoritative-sources-in-a-hyperlinked-environment.pdf) [Authoritative Sources in a Hyperlinked Environment](https://www.cs.cornell.edu/home/kleinber/auth.pdf)(超链接环境中的权威来源)- Jon M. Kleinberg

  这篇论文提出了 **HITS 算法**——一种对网页进行评级的链接分析算法。与更有名的 PageRank 不同,HITS 算法对网页行为加以区分,把它们分类为 hub(枢纽)与 authority(权威)。一个页面要么是权威页面(拥有大量入链),要么充当枢纽(某种目录,可用出链数量衡量)。HITS 为每个页面计算两个分数(权威分与枢纽分):算法迭代地把枢纽分计算为其出链页面权威分之和、把权威分计算为其入链页面枢纽分之和,直到收敛。这些分数随后可用于文档排序。该算法在学术界很有名,但工业界使用并不广泛(Teoma 公司曾使用它的一个变体,该公司后来被 AskJeeves 收购)。
