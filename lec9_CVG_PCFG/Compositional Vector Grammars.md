 Compositional Vector Grammars
--
CVG模型主要是用来将一个句子映射到一个与词相同的向量空间的模型。CVG是一个结合了PCFG（概率上下文无关）和RNN（递归网络）各自优点的模型，PCFG能够将短语划分到某一离散的类别（如NP，VP），RNN能够捕获到短语的详细信息，某些具有二义性的语法可以通过语义来消除二义性，如They ate udon with forks. vs. They ate udon with chicken。也就是说，CVG能够同时捕获短语的语法结构和不同结构所表达的信息。
Probabilistic Context Free Grammar
--
PCFG主要是用来构建具有二义性文法的语法树的算法，在使用CFG模型对某个具有歧义的句子构造语法树时，往往可以构建出多棵语法树，PCFG正是用来解决此问题的
