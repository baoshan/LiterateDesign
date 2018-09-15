# 概览

文学化设计（Literate Design）是一种产品设计思路。文学化设计鼓励以叙述式的风格，通过自然语言与文本文档的合理使用，实现更加朴素的产品体验。

# 文学化设计的特性

文学化设计常常包括以下8种特征：

1. 能讲普通话 —— 通过自然语言呈现事实；
2. 会读普通话 —— 通过自然语言定义数据；
3. 听懂普通话 —— 通过自然语言发起操作；

4. 功能内容化 —— 通过自然语言定义人、机行为；
5. 界面文档化 —— 避免“控件海”风格的界面设计；
6. 架构路径化 —— 通过文件夹显式表达信息架构；

7. 研发文学化 —— 文学化设计驱动的研发流程；
8. 始终同步 —— 内容、流程与工具的始终同步。

这些特征的总结，单纯为了启发设计师理解文学化设计的内涵。对于某个具体案例，并不需要刻意涵盖全部特性。下面，分别阐述这些特性。

## 1. 能讲普通话

文学化设计鼓励通过自然语言呈现事实。

产品设计师通过词法（Lexicology）与语法（Grammar）这两个层级，逐步达成「能讲普通话」的基本目标。

首先，根据目标场景的专业程度，用满足目标场景沟通需求的朴素词汇替代生僻词汇，使得界面与用户的沟通方式是文学化、易读的，例如：

| 目标场景 | 好词汇 | 坏词汇 |
|:--|:--|:--|
| 《柳叶刀》 | cerebral | brain |
| 医患沟通 | brain | cerebral |
| 几乎任何场景 | 手机 | 便携式移动智能终端 |
| 几乎任何场景 | 编号 | ID号 |

其次，文学化设计鼓励使用叙述性的自然语言沟通事实，而非通过以界面控件（标签、文本框、列表、日历控件、按钮，等）承载的碎片信息，由用户「脑补」事实。

例如：文学化设计倾向于呈现「苏丽珍预约下周二体检」，而非：

![使用界面控件呈现事实](/assets/1.1.png)

文学化设计倾向于呈现「林智明医生周三上午在中医科出诊」，而非：

![使用界面控件呈现事实](/assets/1.2.png)

## 2. 会读普通话

文学化设计鼓励通过自然语言定义数据。

「会读普通话」是「能讲普通话」的反函数。如果除周三上午之外，林智明医生增加周五全天出诊。文学化设计的产品，用户仅需将「林智明医生周三上午在中医科出诊」修改为「林智明医生周三上午和周五全天在中医科出诊」；而非通过一系列的界面控件交互（按钮点击、列表点选、拖拽，等），达到下图效果：

![使用界面控件定义数据](/assets/2.1.png)

对于企业应用，多数用户期待系统的行为具有较高的可预测性，并愿意为此接受培训。现阶段，基于规则与模式匹配的自然语言处理算法更适宜企业应用。作为辅助，机器学习算法可用于纠正拼写与语法错误等。

## 3. 听懂普通话

文学化设计鼓励通过自然语言发起操作。

对于语音交互、聊天机器人等渴望即时响应（同时对上下文依赖较弱）的场景，用自然语言发起操作，符合用户预期。例如：如果希望将苏丽珍下周二的体检预约改到下周五，用户可以这样发起请求：

![使用自然语言发起操作](/assets/3.1.png)

这里的「听」，并不要求系统可以直接响应语音输入——能够处理（基于自然语言的）文字请求，通常是「听懂普通话」的第一步。

## 4. 内容即功能

文学化设计鼓励通过自然语言定义人、机行为。

设计师通过三个层次实现「内容即功能」：

1. 通过自然语言定义系统行为；
2. 通过自然语言定义用户行为；
3. 通过丰富语义进化人机行为。

用自然语言定义系统行为，指：系统行为与（存在于文本文档中的）用于定义系统行为的自然语言实时同步。例如：通过撰写「下周一起，金额大于1,000元的线上订单，需由餐厅经理审核」来定义和调整系统行为；而非通过类似下图的界面控件交互，达成诉求：

![使用界面控件定义行为](/assets/4.1.png)

对企业应用而言，除了通过自然语言定义系统行为之外，还需要使用自然语言定义用户行为，以便向客户交付标准化产品或服务。在撰写时，系统行为与用户行为无需在文件级别加以区分，而应当按照为阅读者优化的信息架构进行组织。用于定义用户行为的内容，因为系统无需解读与执行，行文空间较大；除此之外，在撰写时并无其它区别。

通过丰富语义进化系统行为，指：当新需求产生时，设计师通过丰富系统可以理解的自然语言语义，来完成用户诉求。例如：当系统需要为出诊医生分配诊室时，文学化设计的产品，用户仅需将「林智明医生周三上午在中医科出诊」修改为「林智明医生周三上午在中医科出诊，使用107诊室」，而非由界面设计师增加额外的界面控件（如：标签、列表）来达成诉求。

## 5. 文档即界面

文学化设计鼓励使用文本文档作为人机界面，避免“控件海（Oceans of Controls）”风格的界面设计。

与文档化界面设计相对的，是控件化界面设计。控件化界面设计根据逻辑模型（或更糟糕的情况：物理模型）选择、排列界面控件，用户通过操纵这些控件，来满足设计师（或更糟糕的情况：工程师）的需求。文学化设计中，用户通过用自然语言描述数据（内容）与行为（流程），文本文档作为自然语言的优质载体，自然而然地成为了用户界面的优选方案之一。

文本文档中需要机器解析的部分，可以用Markdown语法、RTF语法，或DSL语法撰写。在满足可读性的同时，方便机器解读。

例如，文学化设计倾向于使用一个命名为「医生门诊出诊时间.md」的文档，包含以下内容：

	目前，我院医生门诊出诊时间安排如下：
	
	1. 林智明医生周三上午在中医科出诊
	2. 徐亮医生周一至周五全天在男科出诊

这样「文档即界面」的设计，优于部分采用文学化设计，部分采用界面控件的方案：

![部分采用文学化设计](/assets/5.1.png)

又例如，文学化设计倾向于使用一个命名为「食品价格与库存位置.md」的文档，包含以下内容：

	| Product         | Price | Location |
	|:----------------|------:|---------:|
	| Meiji Chocolate |  6.00 |     22-5 |
	| New York Cheese | 12.00 |      3-8 |

取代使用网格控件绘制的界面：

![使用网格控件](/assets/5.2.png)

又例如，文学化设计倾向于使用一个命名为「周慕云.md」的文档，包含以下内容：

	身份证号：110101204611222229

取代使用界面控件绘制的界面：

![使用界面控件](/assets/5.3.png)

用户通过保存文本文档，完成对数据或行为的调整，取代以按钮提交表单的方式。

## 6. 架构路径化

文学化设计通过自然语言作为信息的载体，描述数据（内容）与行为（流程）。信息设计是文学化设计的最重要环节。而信息架构设计，又是信息设计的首要步骤。

文件夹（层级式结构）是信息架构的载体，设计师会用很多的时间进行文件夹设计。

此处，「文件夹设计」并非指视觉呈现上需要与图形化文件操作系统内建的文件夹样式一致；而是指设计师与用户的思维模式，与文件系统一致 —— 系统的状态完全取决于（函数依赖于）文件内容与文件结构。

与文学化设计背道而驰的，是使用导航与菜单来承载信息架构。文学化设计不鼓励这样的实现途径：

![使用导航或菜单承载信息架构](/assets/6.1.png)

## 7. 研发文学化

当文学化设计被应用到极致之后，研发流程会发生改变——产品设计与研发将按如下方式分工：

1. 设计师用自然语言来撰写文档，同时设计适合的架构来组织信息；
2. 工程师研发编译器来解析文档，将文档编译成机器可执行的代码。

项目干系人可以通过阅读这些自然文档，随时了解产品研发进度。

## 8. 始终同步

文学化设计的「工具」（信息系统），使用自然语言与文本文档作为信息载体，唯一地、无歧义地定义并管理「流程」与「内容」，达到「流程」、「内容」、「工具」这三者全生命周期始终同步的目的。

大中型企业，核心业务均由多部门协同完成。因为管理水平低、设计能力低、责任心缺失、沟通不充分、外部环境不稳定等因素，很容易造成企业「流程」（人与系统的动态行为标准）、「内容」（需要存储与呈现的静态信息）与「工具」（信息系统）的不同步，直接影响运营表现。

大多数产品在首次交付时，缺少用户可以理解的、文学化的，而非（抽象）形式化的系统行为定义。随着业务的进化与产品的迭代，更无可避免地会出现文档（需求文档、设计文档、用户手册等）与实际产品不同步的问题。

通过自然语言定义人、机行为，保证了在产品的全生命周期内，用户通过阅读、撰写、编辑基于自然语言的文档内容、文档结构、文件夹结构，即可理解、控制系统的实时行为。文档（需求文档、设计文档、用户手册等）与实际产品始终同步。

## 文学化设计的灵感

**屏幕阅读器**

设想一下：用户在刚刚接触一个大量、不规则使用传统控件的界面（比如：由超过20个文本框、标签、下拉列表、按钮等传统控件构成的表单）时，他的感觉，和一个有视觉障碍，只能使用屏幕阅读器来操作界面（尤其是没有为屏幕阅读器优化过的界面）的用户多么地相似——单词、元数据、停顿、错位的语序构成了用户的全部体验。

在现实中，有相当多的表单超出了这个复杂度。我熟悉的两个领域：音乐元数据管理、医院信息化都充满了“控件海（Oceans of Controls）”的负面案例。

合理应用文学化设计之后，对于视觉正常的用户而言，可以更快、更自然、更少歧义地理解信息；对于有视觉障碍的用户，可以获得比单纯为屏幕阅读器优化界面更好的体验。

可以认为：文学化设计，使用了为视觉障碍用户的设计产品的技巧，为没有视觉障碍的用户优化产品。

**编译器**

大部分自然语言有着足够丰富和准确的语义，可以用于定义信息系统的行为和数据。但是自然语言机器无法执行，这之间空缺的部分就是领域特定编译器（Domain-Specific Compiler）。

可以认为：文学化设计，通过编译器设计的思路，设计自然语言的编译器。

**界面与语言**

我们经常认为：界面是人与机的边界，是有机生命体与算法、算力、数据与带宽的边界。

可以认为：文学化界面是机器语言与自然语言的边界，是用户思维模式与工程师思维模式的边界。

## 文学化设计不是什么

**文学化设计不是榔头**

文学化设计是产品设计师的一种工具，而不是一种强制性的产品设计风格。很多时候，当产品设计师的思维模式固化在传统交互控件上时，往往会忽略掉更好的方案。应用文学化设计，仍然需要产品设计师仔细分析每个场景、功能点的特殊性，最终决定：是否通过文学化设计来解决面对的问题。

文学化设计是产品设计师的一个工具，不要拿着榔头，看到的所有东西都变成了钉子。避免「为了文学化设计而文学化设计」这类刻意生搬硬套的情况的发生。

**文学化设计不是无控件设计**

文学化设计的构思，受到过极简主义设计师（例如：Dieter Rams）的影响。成功地应用文学化设计，虽然可以减少界面控件的不必要应用，但是文学化设计并非旨在消灭界面控件的极端主义，而仅仅是为了重新唤起设计师与用户进行（基于自然语言的）叙述性沟通的意识。

合理应用文学化设计之后，绝大多数界面与交互设计仍需适度使用界面控件。

**文学化设计不是文档型数据库**

虽然文学化设计通过高可读性的文本内容（自然语言，文本文件、Markdown文件，以及业务人员可读的领域专用语言）来描述信息、定义系统行为，或发起操作，但是应用文学化设计的界面与交互设计并不要求依赖于文档型数据库。根据业务特性：关系型数据库、键–值数据库，甚至Git版本库，都可以做为数据库（或数据持久层）。在进行产品技术架构实践时，文档型数据库与其他数据库技术相比，并无任何优势，亦无任何劣势。

关系型数据库是基于关系理论而构建的数据库管理系统。但是沿用关系型数据库的产品，对用户体验造成的伤害持续存在着，比如：

1. 先从「档案管理/患者管理」查找到「门诊号」；
2. 再到「门诊接诊」界面输入「门诊号」。

## 文学化设计的技术基础

文学化设计，可能会应用以下技术（具体技术超出了本文讨论范畴）：

1. 自然语言处理
2. 语音识别与合成
3. 字体排印
4. 编辑器