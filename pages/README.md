<div style="text-align: center;font-size: 14pt; font-weight: bold;">✨👀简单开发你的qt应用，答应我，别再熬夜了，好吗？👀✨</div>

# Sherry简介

Easy Qt For Python（Sherry） 致力于样式跟界面布局之上，力达能够做出一个快速开发的组件库。

> PS: 我想使用PyQt来开发桌面应用的，应该大都是内部的工具开发或者是个人脚本工具的使用，除去喜好终端交互的趣味，
> 谁不想给自己的工具安一个华丽炫酷的界面呢？这样推荐给别人使用也方便一些吧，我知道这个想法很美好，但作为直男的主要来源群体之一，
> 设计跟美化方面远不及程序开发简单，谁能想到一个颜色细微的差别给人带来的感觉都是千差万别？所以sherry应运而生。


言归正传，如果你也对这个项目感兴趣，请参阅贡献守则，灰原需要诸位有识之士共同守护。

- 加群玩耍💡 【246269919】 PyQt 学习

- 加群玩耍💡 【103058392】 sherry 问题反馈

# 友情链接

- 👉国内玩家请访问[码云](https://gitee.com/pymu/sherry)🚩

- 👉点击[使用教程](helper/quick-start/readme.md) 使用教程，快速上手。

- 👉点击[开发文档](development/readme.md)查看我是如何制作eq框架的。

- 👉点击[组件列表](componet/readme.md)查看已实现的组件，从中选择你喜欢的组件进行开发吧。

- 👉点击[Qss样式指南](theme/readme.md) qss 样式设计指南及控件常见的样式。

- 👉点击[Qt示例](https://github.com/PyQt5/PyQt) 大佬的测试样例，可以解决大部分功能问题。

- 👉点击[打包教程](package/readme.md) python应用打包详解。

# 项目结构

    -sherry                 # 项目目录
        |- sherry           # 框架主包
            |- core         # 框架核心类
            |- inherit      # Qt一系列衍生类
            |- resource     # 框架自带的资源文件夹
            | -utils        # 工具类
            | -variable     # 框架全局变量
            | -view         # 框架内部自带的页面原型即视图
        | -build.bat/sh     # 框架打包脚本
        | -LICENSE          # LICENSE说明
        | -MANIFEST.in      # 框架打包辅助说明
        | -README.md        # 辅助说明
        - requirements.txt # 依赖列表
        - setup.py         # 打包入口

