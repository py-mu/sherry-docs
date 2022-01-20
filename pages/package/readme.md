
# python简介


python运行效率问题，一直是语言交锋的主要阵地，对于一般用户所熟知的python其实是CPython解释器。  
CPython在全局GIL的约束下，python基本可以说是线程安全的， 你无需考虑线程额外的内存锁和同步操作。
> 这不是python的特性，如果还是以此夸夸其谈，会让人一下子看穿你的不业余，应该先从CPython的主要解释器及受众面谈利弊，  
> 然后再抨击python的解释器执行效率低下，记住是解释器不要说python，然后再罗列其他解释语言的性能比，比如js的v8。🤣

这样带来好处同时也给性能上带来很大的灾难，使得大家去视图拆分和去除GIL时，发现python的大量库都非常重度的依赖这个GIL，不是因为去不掉，而是代价过于沉重。
python2到python3已经经历了一个异常艰难的过渡（重点来了，又是一个交锋的阵地，python不能向下兼容，就是python2的代码，
不能在python3中运行）。而现存的python库大都重度依赖这GIL，牵一发而动全身，不过目前python也在尝试解决问题，除了全局锁，python的解释效率差强人意。

>为此python社区也针对解释器衍生出众多流派，其中CPython自持正统，除了CPython之外还有IPython、PyPy、Jython、IronPython等等，
>其中IPython以科学计算、友好的阅读性出众，原生的IPython，可能用的比较少，但是提及jupyter note，学过python的都应有所耳闻，但其本身还是CPython的扩展。
>说道性能就不得不谈PyPy了，说他是解释器其实也不算，因为他是一种JIT编译器，想要了解的可以私下里扩展。

除了解释器，还有编译器，即对python代码进行编译后再运行，从本质上解决python运行效率低下的问题。python常用的编译器就只有两个：

- LLVM后端的numba
- 支持大部分C++编译器作为后端的nuitka

参考链接：
1. [python 两大编译器numba与nuitka有何区别](https://www.zhihu.com/question/387301789)
2. [如何看待 PyPy 与 Pyston 的未来？](https://www.zhihu.com/question/50514698)
3. [python 3.6与JIT特性](https://docs.python.org/3.6/whatsnew/3.6.html#pep-523-adding-a-frame-evaluation-api-to-cpython)
4. [numba从入门到精通（1）—为什么numba能够加速](https://zhuanlan.zhihu.com/p/68720474)
5. [全新模式的 Python JIT—— Pyston v2](https://zhuanlan.zhihu.com/p/142059317)
6. [PyPy 为什么会比 CPython 还要快？](https://www.zhihu.com/question/19588346)


