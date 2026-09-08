> 🌐 本文档由 [papers-we-love/papers-we-love](https://github.com/papers-we-love/papers-we-love) 翻译,英文原版见原项目。
>
> 注:论文标题保留英文原名以便检索原文,全部链接保持原样;说明文字已译为中文。

# Haskell

* [A History of Haskell: Being Lazy With Class](http://research.microsoft.com/en-us/um/people/simonpj/papers/history-of-haskell/history.pdf)(Haskell 史: 慵懒而有格调),Paul Hudak、John Hughes、Simon Peyton Jones
* :scroll: [Tackling the Awkward Squad: monadic input/output, concurrency, exceptions, and foreign-language calls in Haskell](tackling-the-awkward-squad-monadic-input-output-concurrency-exceptions-and-foreign-language-calls-in-haskell.pdf)(搞定"难缠一伙": Haskell 中的单子 I/O、并发、异常与外部语言调用),Simon Peyton Jones
* :scroll: [Making a Fast Curry: Push/Enter vs. Eval/Apply for Higher-order Languages](making-a-fast-curry-push-enter-versus-eval-apply-for-higher-order-languages.pdf)(Making a Fast Curry: 高阶语言的 Push/Enter 与 Eval/Apply 之争),Simon Marlow 与 Simon Peyton Jones。经典之作……清晰描述了 GHC 执行 Haskell 程序所用的执行模型,并记录了两位天才作者如何依据实证数据,把设计思路从最初的直觉转向了新的结论。
* :scroll: [A Poor Man's Concurrency Monad](a-poor-mans-concurrency-monad.pdf)(穷人的并发单子),Koen Claessen。这篇论文描述了如何在不给语言增加任何原语的情况下,在 Haskell 中定义一个并发单子变换器。
* :scroll: [Parallel Generational-Copying Garbage Collection with a Block-Structured Heap](../../garbage_collection/parallel_generational_copying_garbage_collection_with_a_block_structured_heap.pdf)(块结构堆上的并行分代复制垃圾回收)。在 Haskell 中,数据不可变性迫使我们产生大量临时数据,但同时也帮助这些垃圾被快速回收。这篇论文解释了 Glasgow Haskell Compiler 如何以简单而有效的方式、无需程序员干预地完成这项任务。
* [Notions of Computation and Monads](https://core.ac.uk/download/pdf/82259574.pdf)(计算的概念与单子),Eugenio Moggi。函数式范式中关于单子(Monad)的经典文献之一。它把计算的语义与各种计算概念下的程序等价性联系起来。
* [The Essence of Functional Programming](https://page.mi.fu-berlin.de/scravy/realworldhaskell/materialien/the-essence-of-functional-programming.pdf)(函数式编程的精髓),Philip Wadler。这篇论文用单子来组织 Haskell 函数式程序。无论是理解单子本身,还是放在更广泛的编程语言语境下,它都是非常好的参考文献。
* [Monad Transformers and Modular Interpreters](https://dl.acm.org/doi/pdf/10.1145/199448.199528)(单子变换器与模块化解释器),Sheng Liang、Paul Hudak 与 Mark Jones。关于单子变换器(Monad Transformer)的权威论文:它是组合单子的标准方法,也是流行的 Haskell mtl 库的基础。
* [Extensible Effects: An Alternative to Monad Transformers](http://okmij.org/ftp/Haskell/extensible/exteff.pdf)(可扩展效果: 单子变换器的替代方案),Oleg Kiselyov、Amr Sabry 与 Cameron Swords。一篇有影响力的立场论文,引入代数效应(algebraic effects)作为单子变换器的替代。效果通过效果集合的类型级 Open Union(每种效果一个)建模,并以 Free Monad 解释代数效应。它是 extensible effects 库的基础。
* [Freer Monads, More Extensible Effects](http://okmij.org/ftp/Haskell/extensible/more.pdf)(更自由的 Free Monad,更可扩展的效果),Oleg Kiselyov 与 Hiromi Ishii。对 extensible-effects 库的扩展,移除了 Free Monad 类型上的 Functor 约束。
* [Data types a la carte](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/14416CB20C4637164EA9F77097909409/S0956796808006758a.pdf/data-types-a-la-carte.pdf)(Data types à la carte: 按需点菜的数据类型),Wouter Swierstra。一篇广受欢迎的论文,利用智能构造器与注入算子解决 Wadler 的表达式问题。它也是通过效果 Functor 开发代数效应的经典方法,参见下文 Wu、Shrijvers 与 Hinze 的工作。
* [Effect Handlers in Scope](http://www.cs.ox.ac.uk/people/nicolas.wu/papers/Scope.pdf)(作用域内的效果处理器),Nicolas Wu、Tom Shrijvers 与 Ralf Hinze。关于开发代数效应与"à la carte"效果处理器的非常有意思的论文。它通过引入高阶语法来处理效果之间的交互(例如状态与异常,其中错误会回滚状态),扩展了 Swierstra 的工作。
* [Fusion for Free: Efficient Algebraic Handlers](https://people.cs.kuleuven.be/~tom.schrijvers/Research/papers/mpc2015.pdf)(免费的融合: 高效代数处理器),Nicolas Wu 与 Tom Shrijvers。在"把带效果的计算视为 Free Monad 抽象语法树、把处理器视为 fold"的解释之下,这篇论文引入 Term Monads 来实现 fold 融合。处理器随后可以合并为单个 fold 并被 GHC 内联,从而获得与 extensible effects 和 mtl 库相当、某些情况下甚至更优的性能(附证明与测试)。
* [Handlers In Action](http://homepages.inf.ed.ac.uk/slindley/papers/handlers.pdf)(Handlers In Action: 实战中的效果处理器),Ohad Kammar、Sam Lindley 与 Nicolas Oury。一篇有影响力的立场论文,也是开发代数效应与处理器的 Haskell 库的基础。该模板 Haskell 库使用类型族(type families)而非 à la carte 的余积函子来支持开放处理器。
* [Composing Fractals](http://web.cecs.pdx.edu/~mpj/pubs/composing-fractals.pdf)(组合分形),Mark P. Jones。这篇论文描述了一族简单而灵活的 Haskell 程序,用于绘制 Mandelbrot 集与 Julia 集等分形图形。其主要目标是展示组合式程序构建方法的优雅,以及程序行为各侧面之间清晰分离所带来的好处。
