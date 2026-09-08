# papers-we-love 中文文档

[![原项目](https://img.shields.io/badge/原项目-papers--we--love--papers--we--love-blue?style=flat-square&logo=github)](https://github.com/papers-we-love/papers-we-love)
[![微信联系](https://img.shields.io/badge/微信-uaycar-brightgreen?style=flat-square&logo=wechat)](#)

> 本文档是 [papers-we-love/papers-we-love](https://github.com/papers-we-love/papers-we-love) 的中文翻译介绍,原项目与全部论文版权归 Papers We Love 社区及各论文作者所有。

## 项目简介

**Papers We Love**(*PWL*)是一个以阅读、讨论和学习计算机科学学术论文为核心的社区。这个仓库相当于一份精选论文目录,把散落在网络各处的优秀学术文档汇聚到一起。由于内容许可(license)的限制,仓库并不总是能直接托管论文原文——凡是能托管的,目录中会在论文标题旁标注 📜 表情,其余则提供原始链接。

除了 GitHub 仓库,你还可以:

- 访问 [Papers We Love 官网](http://paperswelove.org/) 了解更多信息;
- 加入各地分会(Chapter)的线下聚会,参与现场讨论;
- 在官方 [Discord 服务器](https://discord.gg/Tu2VynkRWv)讨论 PWL 活动与仓库内容;
- 在 [YouTube 频道](https://www.youtube.com/user/PapersWeLove)观看历届分享会视频。

所有聚会均遵循原项目的 [Code of Conduct(行为准则)](https://github.com/papers-we-love/papers-we-love/blob/main/CODE_OF_CONDUCT.md)。想在自己的城市发起分会,请参考 [organizers 仓库](https://github.com/papers-we-love/organizers)。

## 内容组织

原仓库的论文按计算机科学的主要方向分类存放于 `papers/` 目录,典型方向包括:

- **分布式系统**:如 Paxos、Raft、Spanner、Dynamo 等经典系统论文;
- **数据库**:存储引擎、查询优化、事务一致性等方向的基础论文;
- **编程语言与编译器**:类型系统、函数式编程、运行时实现等;
- **操作系统与网络**:调度、虚拟化、拥塞控制、协议设计等;
- **其他方向**:机器学习、安全、硬件、体系结构等,持续扩充中。

每篇论文在目录中附带标题、作者与链接(部分含可下载的 PDF),具体清单以原仓库为准。

## 如何阅读论文

读论文不等同于读博客或小说,原项目整理了一批入门资料:

- [How to read an academic article](http://organizationsandmarkets.com/2010/08/31/how-to-read-an-academic-article/) — 如何阅读学术文章
- [Advice on reading academic papers](https://userpages.umbc.edu/~akmassey/posts/2012-02-15-advice-on-reading-academic-papers.html) — 阅读学术论文的建议
- [How to read a paper](http://ccr.sigcomm.org/online/files/p83-keshavA.pdf) — 经典三遍读论文法(S. Keshav)

建议从"三遍读法"入手:第一遍快速扫清标题、摘要、结论,判断是否值得读;第二遍弄清图表、方法与论证主线;第三遍在头脑中"复现"论文工作。

## 下载论文

打开终端,在仓库根目录运行:

```bash
$ ./scripts/download.sh
```

该脚本会抓取 Markdown 目录中的 PDF 链接,并把论文下载到各自的目录下。更多用法与选项见原仓库 [scripts/README.md](https://github.com/papers-we-love/papers-we-love/blob/main/scripts/README.md)。

## 更多找论文的好地方

原 README 还列出了大量论文检索资源,代表性条目包括:

- [arXiv 论文库](http://arxiv.org/) — 计算机科学预印本主站
- [alphaXiv](https://www.alphaxiv.org/) — 为 arXiv 论文叠加讨论层
- [Google Scholar](http://scholar.google.com/citations?view_op=top_venues&hl=en&vq=eng) — 按子领域查看顶级期刊/会议
- [The Morning Paper](http://blog.acolyer.org/) — 经典论文的短评博客
- [2 Minute Papers](https://www.youtube.com/user/keeroyz) — 视频化论文讲解
- [Microsoft Research](https://www.microsoft.com/en-us/research/publications/) 与 [Facebook Research](https://research.facebook.com/publications/) — 工业界论文库

完整清单与 wiki 页面请见原仓库。

## 参与贡献

原项目欢迎以下方向的 Pull Request:推荐值得收录的新论文、改进现有论文的组织方式、补充其他优质论文仓库链接。详见原项目 [CONTRIBUTING.md](https://github.com/papers-we-love/papers-we-love/blob/main/.github/CONTRIBUTING.md)。

## 版权说明

"Papers We Love" 名称与组织 Logo 的版权归 Papers We Love Ltd 所有,保留所有权利;仓库中各论文的版权归各自作者与出版方所有。发起分会使用 Logo 前请先与官方确认。

---

**代部署 / 定制服务 / 技术咨询 请添加微信:uaycar**

本项目为 [papers-we-love/papers-we-love](https://github.com/papers-we-love/papers-we-love) 的中文翻译介绍,不包含原项目源代码,如对你有帮助请给原项目点个 Star ⭐
