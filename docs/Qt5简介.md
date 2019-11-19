<!-- MDTOC maxdepth:6 firsth1:1 numbering:0 flatten:0 bullets:1 updateOnSave:1 -->

- [Qt 简介](#qt-简介)   
   - [Qt发展](#qt发展)   
   - [Qt功能特性](#qt功能特性)   
   - [Qt工具集](#qt工具集)   
   - [参考](#参考)   

<!-- /MDTOC -->
# Qt 简介

![20191025_201612_13](image/20191025_201612_13.png)

**Qt 本质是C++写的GUI开发框架**，使用 Qt 只需一次性开发应用程序，无须重新编写源代码，便可跨不同桌面和嵌入式操作系统部署这些应用程序。

**Qt 主要用于桌面程序开发和嵌入式开发**

官方站点:<https://www.qt.io/>


## Qt发展

Haavard Nord和Eirik Chambe-Eng于1991年开始开发“Qt”，1994年3月4日创立公司，最早名为Quasar Technologies，然后更名为Troll Tech，然后再改为Trolltech，中文名是“奇趣科技”，2008年6月17日被NOKIA公司收购，以增强该公司在跨平台软件研发方面的实力，更名Qt Software。

该工具包名为Qt是因为字母Q在Haavard的Emacs字体特别漂亮，而“t”代表“toolkit”，灵感来自Xt，X toolkit。

2009年5月11日，诺基亚Qt Software宣布Qt源代码管理系统面向公众开放，Qt开发人员可通过为Qt以及与Qt相关的项目贡献代码、翻译、示例以及其他内容，协助引导和塑造Qt未来的发展。为了便于这些内容的管理，Qt Software启用了基于Git和Gitorious开源项目的Web源代码管理系统。

在推出开放式Qt代码库的同时，Qt Software在其网站发布了其产品规划（Roadmap）。其中概述了研发项目中的最新功能，展现了现阶段对Qt未来发展方向的观点，以期鼓励社区提供反馈和贡献代码，共同引导和塑造Qt的未来。2012年8月9日，Digia宣布已完成对诺基亚Qt业务及软件技术的全面收购，并计划将Qt应用到Android、iOS及Windows 8平台上。


**Qt 命运多舛，总共经历了三家公司**

1. Qt 由奇趣科技公司（Trolltech）的两位创始人于1990年着手开发，1995年发布Qt  1.0。
2. 2008年，奇趣科技被诺基亚公司收购，Qt 也因此成为诺基亚旗下的编程语言工具。
3. 在智能手机的冲击下诺基亚大厦轰然倒塌，2012年将 Qt 转让给Digia公司。




## Qt功能特性

* 直观的 C++ 类库：模块化 Qt C++ 类库提供一套丰富的应用程序生成块 (block)，包含了构建高级跨平台应用程序所需的全部功能。具有直观，易学、易用，生成好理解、易维护的代码等特点。
* 跨桌面和嵌入式操作系统的移植性：使用 Qt，您只需一次性开发应用程序，就可跨不同桌面和嵌入式操作系统进行部署，而无须重新编写源代码，可以说Qt无处不在（QtEverywhere） 。
* 使用单一的源代码库定位多个操作系统；
* 通过重新利用代码可将代码跨设备进行部署；
* 无须考虑平台，可重新分配开发资源；
* 代码不受担忧平台更改影响的长远考虑 ；
* 使开发人员专注于构建软件的核心价值，而不是维护 API 。
* 具有跨平台 IDE 的集成开发工具：Qt Creator 是专为满足 Qt 开发人员需求而量身定制的跨平台集成开发环境 (IDE)。Qt Creator 可在 Windows、Linux/X11 和 Mac OS X 桌面操作系统上运行，供开发人员针对多个桌面和移动设备平台（IOS, Andoid等）创建应用程序。
* 在嵌入式系统上的高运行时间性能，占用资源少。

## Qt工具集

* Qt Creator：轻量级的Qt/C++ IDE开发环境。
* qmake：跨平台构建工具，可简化跨不同平台进行项目开发的构建过程。
* Qt Designer：界面设计师。可以用拖拽的方式将Widget排放在界面上，支持版面配置，支持信号与槽编辑。
* Qt Assistant：Qt助手。Qt在线帮助文件查看工具。
* Qt Liguist：翻译工具。读取翻译文件（如.ts、.po）并为翻译人员提供友好的翻译接口。
* lupdate：从源代码文件或其他资源文件中提取需要翻译的字符串，并将之存入xml格式的.ts文件中。
* lrelease：负责将.ts文件转化为程序使用的.qm文件。.qm档会去掉.ts档中所有的空白和未翻译的内容，并将存储格式压缩。
* lconvert：用于翻译文件之间的格式转换。
* QVFb：虚拟帧缓存设备，模拟framebuffer设备（尺寸、色深），还可以透过skin模拟硬件键盘的布局（包括特殊的按键），可以便捷在桌面系统机器上开发嵌入式程序
* makeqpf：创建用于嵌入式设备的qpf格式。qpf是一种预先渲染的字体，直接保存成二进制内容，使用的时候可以用存储器映射加载，从加载到绘制的过程不需要计算。
* uic：User Interface Compiler。从用户界面的文件（.ui）生成C++代码。
* rcc：Resource Compiler。rcc工具根据.qrc文件的内容将相关的资源在编译过程中嵌入到Qt应用程序。
* qtconfig：基于X11的Qt的配置工具和在线帮助。
* qconfig：Qt Embedded（Linux和Windows CE）配置工具。
* qtdemo：Qt的实例和示范项目的加载器。
* qt3to4：协助移植Qt 3程序到Qt 4的工具。
* qdbusxml2cpp：QtDBus XML compiler。将xml格式的D-Bus接口描述转换成为C++源代码
* D-Bus Viewer：可以查看D-Bus对象和信息的工具。
* Qt Visual Studio Add-in：Visual Studio集成
* Qt Eclipse Integration：Eclipse集成


## 参考

* <https://zh.wikipedia.org/wiki/Qt>

---
