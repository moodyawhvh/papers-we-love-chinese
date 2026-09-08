> 🌐 本文档由 [papers-we-love/papers-we-love](https://github.com/papers-we-love/papers-we-love) 翻译,英文原版见原项目。
>
> 注:论文标题保留英文原名以便检索原文,全部链接保持原样;说明文字已译为中文。

### 渲染(Rendering)

* :scroll: [Digital Video Stabilization and Rolling Shutter Correction using Gyroscopes](http://graphics.stanford.edu/papers/stabilization/karpenko_gyro.pdf)(用陀螺仪做数字视频防抖与卷帘快门校正)
这是一篇非常出色的论文,既复杂又直白。论文"提出了一种基于陀螺仪的鲁棒实时视频防抖与卷帘快门校正技术"。老子认为它了不起的地方在于:巧妙利用了大众化技术(智能手机的陀螺仪),通过实时消除视频抖动和卷帘快门伪影,给手机的核心部件——摄像头——带来了最先进的改进。

* [An Improved Illumination Model for Shaded Display](https://www.cs.drexel.edu/~david/Classes/CS586/Papers/p343-whitted.pdf)(一种改进的明暗显示光照模型,即 Whitted 光线追踪)

* [GigaVoxels : Ray-Guided Streaming for Efficient and Detailed Voxel Rendering](http://maverick.inria.fr/Publications/2009/CNLE09/CNLE09.pdf)(GigaVoxels: 光线引导的流式传输,实现高效精细的体素渲染) - [网页](http://maverick.inria.fr/Publications/2009/CNLE09/) - [项目页](http://gigavoxels.imag.fr/) - [视频](https://www.youtube.com/watch?v=HScYuRhgEJw)

* [Continuous shading of curved surfaces](http://page.mi.fu-berlin.de/block/htw-lehre/wise2015_2016/bel_und_rend/skripte/gouraud1971.pdf)(曲面的连续着色,即 Gouraud 着色),Henri Gouraud(1971)

* [Illumination for computer generated pictures](http://users.cs.northwestern.edu/~ago820/cs395/Papers/Phong_1975.pdf)(计算机生成图形的光照,即 Phong 光照模型),Bui Tuong Phong(1975)

* [The Rendering Equation](http://www.cs.rpi.edu/~cutler/classes/advancedgraphics/S08/lectures/kajiya.pdf)(渲染方程),James T. Kajiya(1986)

### 表面重建(Surface reconstruction)
* [Poisson surface reconstruction](http://research.microsoft.com/en-us/um/people/hoppe/poissonrecon.pdf)(泊松表面重建) - [代码](http://www.cs.jhu.edu/~misha/Code/PoissonRecon/Version5.71/)

* [KinectFusion: Real-time 3D Reconstruction and Interaction Using a Moving Depth Camera](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/kinectfusion-uist-comp.pdf)(KinectFusion: 用移动深度相机进行实时 3D 重建与交互)

### 物体建模(Object modeling)
* [3-Sweep: Extracting Editable Objects from a Single Photo](http://www.cs.tau.ac.il/~dcor/articles/2013/3-Sweep-Extracting-Editable-Objects.pdf)(3-Sweep: 从单张照片中提取可编辑物体) - [视频](https://www.youtube.com/watch?v=Oie1ZXWceqM)

### 照片编辑(Photo editing)
* [Deep Photo Style Transfer](https://arxiv.org/pdf/1703.07511.pdf)(深度照片风格迁移)(2017) - [代码](https://github.com/luanfujun/deep-photo-styletransfer) - 一种基于深度学习的照片风格迁移方法(即把一张照片的风格自动套用到另一张上)。这篇论文里的图片美得惊人。

### 光照(Lighting)
* [Light Propagation Volumes in CryEngine 3](http://www.crytek.com/download/Light_Propagation_Volumes.pdf)(CryEngine 3 中的光传播体积)

### 凹凸映射(Bump mapping)
* [Interactive Horizon Mapping: Shadows for bump-mapped surfaces](https://www.ppsloan.org/publications/bs.pdf)(交互式地平线映射: 凹凸映射表面的阴影)

### 室内映射(Interior mapping)
* [Interior Mapping: A new technique for rendering realistic buildings](http://www.proun-game.com/Oogst3D/CODING/InteriorMapping/InteriorMapping.pdf)(室内映射: 一种渲染逼真建筑的新技术)

### 程序化建模(Procedural modeling)
* 下面两篇论文都是语法驱动生成这一非传统应用的绝佳示例:
  - [Procedural Modeling of Buildings](http://www.peterwonka.net/Publications/pdfs/2006.SG.Mueller.ProceduralModelingOfBuildings.final.pdf)(建筑的程序化建模)
  - [Instant Architecture](http://www.peterwonka.net/Publications/pdfs/2003.SG.Wonka.InstantArchitecture.high.pdf)(Instant Architecture: 即时建筑)

### 网格编辑(Mesh Editing)
* [PushPull++](http://peterwonka.net/Publications/pdfs/2014.SG.Lipp.PushPull.pdf)

    > 在所有操作 3D 网格的方式中,由 SketchUp 推广的 push/pull(推拉)技术是最容易上手、也最有乐趣的之一。PushPull++ 这篇新论文对该技术做了精细打磨:用非常直白的数学清理了大量边界情况,并解锁了新特性。基于这些简单想法构建 3D 建模工具或程序化网格生成 API 的潜力令人非常兴奋。
    > 论文同时介绍了该技术和作者构建的工具。这里重点谈技术部分,因为它是我在这篇论文中最喜欢的部分。(引自 Ramsey Nasser)

### 图像处理(Image Processing)
* :scroll: [Imaging Vector Fields Using Line Integral Convolution](http://cs.brown.edu/courses/csci2370/2000/1999/cabral.pdf)(用线积分卷积可视化矢量场),Brian Cabral 与 Leith Leedom

### 形状文法(Shape grammars)

* [Shape Grammars and the Generative Specification of Painting and Sculpture](http://shapegrammar.org/ifip/SGBestPapers72.pdf)(形状文法与绘画、雕塑的生成性规约)
  - 一篇开创性论文,催生了图形学乃至更广泛设计领域的许多有趣应用;另见 [shapegrammar.org](http://shapegrammar.org/) 上的文献目录。

### 模拟海洋水面(Simulating Ocean Water)

* [Simulating Ocean Water](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.161.9102&rep=rep1&type=pdf)(模拟海洋水面)
  - 水面模拟与渲染领域的开创性论文。

### 抠图(Matting)

* [Blue Screen Matting](https://graphics.stanford.edu/courses/cs148-09-fall/papers/smith-blinn.pdf)(蓝屏抠图),Alvy Ray Smith 与 James F. Blinn。
* [Bayesian Approach to Digital Matting](https://grail.cs.washington.edu/projects/digital-matting/papers/cvpr2001.pdf)(数字抠图的贝叶斯方法),Yung-Yu Chuang、Brian Curless、David H. Salesin 与 Richard Szeliski。
* [Learning-based Sampling for Natural Image Matting](https://openaccess.thecvf.com/content_CVPR_2019/papers/Tang_Learning-Based_Sampling_for_Natural_Image_Matting_CVPR_2019_paper.pdf)(基于学习的自然图像抠图采样),Jingwei Tang、Yagız Aksoy、Cengiz Oztireli、Markus Gross 与 Tunc Ozan Aydın,苏黎世联邦理工学院迪士尼研究中心。
