# python-3
在IPython下如何将常用模块的目录添加到模块的搜索路径下
 有时候，我们import模块的时候系统找不到模块，那是因为当前的工作目录不是模块所在的目录，或者模块的目录没有被添加到模块的搜索路径下。下面我将分别介绍一下这两种方法。
方法1：使用书签来方便的切换目录 

如上图，一开始我的工作目录是C:\Users\libai，然后使用bookmark将F盘下的某个子目录里的Ch02的书签设置成了Ch02，之后直接cd Ch02就可以切换到F:………Ch02了，然后就可以方便的导入此目录下的模块kNN了。
方法2：添加目录到模块搜索路径下
import sys
sys.path.append('F:\pythonCode/machinelearninginacion\Ch02')
sys.path #可查看到上面的目录已经被添加到了搜索路径下
import kNN #这时候就可以直接加载模块了，无论当前工作目录是哪个。
