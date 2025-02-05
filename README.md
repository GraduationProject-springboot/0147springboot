# [首页查询更多项目](https://github.com/GraduationProject-springboot) 包安装运行


# 0147springboot江理工文档管理系统的设计与实现

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1jqaLe1ECs?p=46)


# 绪论
## 1.1 研究背景
在这个推荐个性化的时代，采用新技术开发一个文档系统来分享和展示内容是一个永恒不变的需求。本次设计的文档管理系统有管理员和用户两个角色。管理员功能有论坛管理，公告管理，资料管理，用户管理等。用户可以注册登录，可以上传资料信息，管理员审核后其他用户就可以进行下载，还可以在论坛里面发信息以及查看相关公告信息。


## 1.2 研究意义
通过网络进行文章的转移展示，可以让用户和管理员都能感受到互联网的魅力，让用户解除了地理的远近的限制和降低欣赏时间的成本。本次开发的文档管理系统具有下面的意义：

第一，现实中租赁场地欣赏文章与互联网办公设备的费用比较起来可谓是天上地下，能有效的节约成本。

第二，用户和管理员都可以通过网络查看，避免了线下来回路费的实际成本。

综上所述，网络展示可以让展示变得更加灵活，是对传统展示模式的突破与变革，对于众多用户以及管理员都有很强烈的吸引力和亲和力，在互联网时代真正实现了多环节的多赢。
## 1.3 研究内容
本文主要对已开发程序进行文档说明，文章从绪论，开发技术，系统分析与设计，系统实现与测试等环节进行程序描述。

绪论：绪论部分主要从课题的背景，课题的意义等角度进行阐述。

开发技术：开发技术部分主要还是介绍开发的平台，使用的技术与开发的语言等内容。

系统分析：系统分析部分主要还是分析系统的运行流程与系统需要具备的功能等进行分析。

系统设计：系统设计主要还是基于系统分析，从系统分析得出的功能进行详细设计和数据库设计。

系统实现：系统实现主要运用开发知识对系统设计的功能进行实现。

系统测试：系统测试主要检测完成开发程序整体运行是否报错，程序运行使用是否可靠。



# 2 开发技术
## 2.1 VUE框架
Vue.js（读音 /vjuː/, 类似于 view） 是一套构建用户界面的渐进式框架。

Vue 只关注视图层， 采用自底向上增量开发的设计。

Vue 的目标是通过尽可能简单的 API 实现响应的数据绑定和组合的视图组件。
## 2.2 Mysql数据库
关于程序的数据结构设计，数据的字段设计，为了更好的、更规范的使用数据库，在数据库里进行了字段的设计挑选。关系型数据库可挑选范围不广，基本上也就是甲骨文公司的Oracle和mysql，微软的SQL SERVER和ACCESS，IBM的DB2数据库，常用的也就5个，根据课题需求，创建的程序进行选择数据库的时候，最重要的一条就是符合课题设计的需要，在五个数据库里可以说都符合，但是从课题的需求具体分析，Oracle明显不合适，维护难，又比较臃肿，课题程序只用到了里面很少一部分，SQL SERVER数据库安装维护方面动不动就需要重装系统，因为操作系统的限制，也不采用SQL SERVER，ACCESS数据库比较简单小巧，但是安全性方面还有语言支持方面比较片面，也不予考虑，DBM数据库接触较少也不考虑，只有MYSQL数据库，社区版完全的不用掏钱，并且是开源，值得信赖，从关系型数据库里挑选到MySQL，是因为完全符合课题需要，而且小巧，基本不占用硬盘的空间，处理性能也可以，这就是选择MySQL数据库作为课题程序所需要的数据库的理由。
## 2.3 Spring Boot框架
Spring Boot 是由 Pivotal 团队提供的全新框架，其设计目的是用来简化新 Spring 应用的初始搭建以及开发过程。该框架使用了特定的方式来进行配置，从而使开发人员不再需要定义样板化的配置。用我的话来理解，就是 Spring Boot 其实不是什么新的框架，它默认配置了很多框架的使用方式，就像 Maven 整合了所有的 Jar 包，Spring Boot 整合了所有的框架。

## 2.4 layui介绍
layui 是一套开源的 Web UI 解决方案，采用自身经典的模块化规范，并遵循原生 HTML/CSS/JS 的开发方式，极易上手，拿来即用。其风格简约轻盈，而组件优雅丰盈，从源代码到使用方法的每一处细节都经过精心雕琢，非常适合网页界面的快速开发。layui 区别于那些基于 MVVM 底层的前端框架，却并非逆道而行，而是信奉返璞归真之道。准确地说，它更多是面向后端开发者，你无需涉足前端的各种工具，只需面对浏览器本身，让一切你所需要的元素与交互，从这里信手拈来。
# 3 系统分析
通过阅读查看之前收集的各种文献资料，了解了程序开发遵循的大体流程。其中系统分析也就是其流程当中的一部分，系统分析也是对所选课题，通过对使用者的调查分析，对同类型课题进行比较分析过程中得出本课题需要具备的功能，此部分也是对所选课题的功能等进行需求分析。
## 3.1可行性研究
开发任何程序都需要提前进行分析，也包括了程序的开发与使用是否可行的分析，通常在可行性分析部分，需要涉及到的内容有经济是否可行，有对开发者开发技术上是否可行的分析，有对使用者运行操作程序是否可行的分析等。

（1）技术可行性

此课题主要用于检验本人的专业知识，检验本人将理论运用于实践的能力。由于本人作为大学生，在大学校园学习了程序开发方面的专业知识，也多次根据学院老师布置的期末作业进行过程序小功能模块的制作与开发，也参与过本专业的课程设计作业，因此本人具备一定高度的开发经验，并在开发技术上，比如Spring Boot这种课堂上学习并实践过的网页技术等有了一定的技术基础，在操作软件的使用上，比如数据库Mysql的操作等都有一定的熟练度。所以，只要配置好开发的相关环境，程序开发就会很快上手。

（2）经济可行性

此次课题主要用于毕业答辩，并不是作为商业程序投入社会使用。运用的开发软件通过各大网页浏览器就可以下载在笔记本电脑上，环境安装教程也在各大网页浏览器上查看，在开发期间，包括代码的编写也可以通过网页浏览器下载相应功能模块的代码，然后对下载的功能模块代码进行相应的编辑，就可以写入程序中。可以说整个过程并没有涉及到资金的投入，在程序开发硬件设备上，仅需一台电脑，鼠标，键盘等设备，这些硬件设备也无需额外掏钱欣赏，因为校园文章馆有专门的计算机机房供学生使用，另外，由于本专业的原因，本人早期已购置一台笔记本，所以硬件设备都已具备。因此此程序在经济投入上是零支出，具备可行性。

（3）运行可行性

此次课题在界面设计上讲究简单化，美观的设计原则，在对各个功能的流程设计上也是比较通俗易懂的，所以程序一旦投入使用，对使用者的计算机操作水平没有过多要求，加上现如今计算机在各个行业都有运用，以及人们学历的普遍提升，大部分人在操作具备可视化操作界面的程序时，很快就可以上手，就算有少数人不懂怎么操作，经人简单指点培训也可以操作程序。因此，程序投入使用，在运行上具备可行性。

程序可行性分析，分析了开发者的技术可行，分析了使用者的运行使用可行，分析了程序开发的经济可行。总之，开发与使用该程序完全可行。
## 3.2系统性能分析
程序一旦开发完成，就会投入生活中使用，使用者大多都是使用程序的功能区解决问题，之所以去分析程序需要具备的性能特征，主要还是确保程序运行中，在质量上是可靠的，在数据安全上是值得放心的，以及程序是一个健壮性的程序，程序在今后的社会变化中，也能通过编辑修改进行升级，以满足使用者不断变化的需求等等，这些特点都是程序的性能需要具备的特点。之所以要进行性能分析，也主要是考虑程序投入使用中，要尽可能降低程序的维护成本，要始终保持程序可以可靠运行，并长时间帮助使用者处理各种数据。在程序的功能符合使用者的要求的前提下，只有稳定可靠的程序，才能得到使用者的青睐。
## 3.3 系统流程分析
每个程序开发出来，不管是登录，添加信息等操作都是遵循一定的操作流程的，每个流程都有相应的判断，所以在分析系统的时候，也有必要对系统的流程进行分析。
### 3.3.1 系统开发流程
程序开发首先需要分析所开发程序的功能，这个步骤也是程序的需求分析阶段，这个阶段的任务很重要，因为程序功能确定之后，后面的设计，编码等环节都跟系统的分析阶段所完成的内容挂钩。程序在开发时大致都遵循以下流程。

![](/md/blog.001.png)

图3.1系统开发流程图
### 3.3.2 系统注册流程
程序提供注册的功能（注册对应流程在下图展示）。就是让非系统操作用户变成程序的操作用户，主要让用户在注册页面上，根据页面提示，规范填写个人信息，程序也会根据用户填写的内容进行逻辑判断，确定用户身份是合格的身份之后，用户填写的数据才可以被数据库写入用户数据表里面。

![](/md/blog.002.png)

图3.2 注册流程图
### 3.3.3 系统登录流程
程序投入生活让使用者使用，都需要经过登录模块这个入门环节，这个功能也就像现实生活一样，需要使用正确的钥匙打开门，才能进入。而登录模块需要的钥匙就是账号，密码，这两项数据正确就能访问程序的功能区。登录流程也会在下图展示，里面也有相应的判断规则。

![](/md/blog.003.png)

图3.3 登录流程图




# 4 系统设计
系统分析接下来的操作步骤就是系统的设计，这部分内容也是不能马虎对待的。因为生活都是在不断产生变化，人们需求也是在不断改变，开发技术也是在不断升级，所以程序也需要考虑在今后可以方便进行功能扩展，完成升级。程序也需要具备大容量以及对其它软硬件的适应能力，而不仅仅是满足现有用户提出来的功能需求，程序在设计期间始终要以发展的理念来进行，要让程序的开发技术上具备先进性的特点，也要让程序开发成本降低，以及让程序后期运行使用时易于维护。
## 4.1 系统结构设计
本程序在设计结构选择上首选B/S，也是为了满足程序今后升级便利，以及程序低维护成本的要求。本程序的网络拓扑设计也会在下图展示，通过图形的方式来描述更容易理解。

![](/md/blog.004.png)图4.1 系统网络拓扑设计图
## 4.2系统功能模块设计
程序的功能在系统分析这部分已经确定了，这部分主要还是针对程序功能进行更加详细的设计，设计成果使用结构图展示直观明了，也更容易让人理解。绘制结构图采用的工具是Visio，使用它可以快速绘制出不同角色拥有的功能结构。

![结构设计图](/md/blog.005.jpeg "结构设计图")

图4.2 功能结构图
## 4.3数据库设计
对程序的功能分析与结构设计之后，也要对程序数据存储的工具进行选择，本程序选用的数据存储仓库是Mysql，选用这个工具就需要根据该数据库的特点进行数据库文件的创建，并设计与之对应的数据表。
### 4.3.1数据库E-R图
设计一个数据库，不仅包含了数据库实体的设计，也包括了数据库表的结构设计，此部分内容设计的就是确认数据库的实体，并在此基础上对每个实体应该有的属性值进行分析设计，这些确认好的属性值对接下来的数据表的设计也是有很大帮助的，因为它们代表数据表里面的字段值。通常每个程序的数据库里面都具备用户这样的一个数据表。那么在分析用户这个实体的时候，都会设计出它的属性，有最基本的登录程序的账号属性，有用户的姓名属性，有用户的电话或联系地址属性等内容。一旦确认实体具备的属性之后，就可以采用相应的设计软件绘画出实体属性图，或者是实体之间的E-R图。设计E-R模型的软件有很多，这里列举常用的几个，一个是PowerDesigner，一个是Navicat绘制E-R模型，本设计模块用到的还是之前课堂上就了解并接触的Visio工具，这个工具跟办公软件Word，Excel一样都属于Office里面的一部分。使用Visio工具不仅在软件安装上快捷高效，而且它不会占用很多计算机的存储空间。

（1）下图是论坛实体和其具备的属性。

![D:\111sheji\文档管理系统\wendangguanli\\img\论坛.jpg](/md/blog.006.jpeg "D:\111sheji\文档管理系统\wendangguanli\\img\论坛.jpg")
论坛实体属性图

（2）下图是用户实体和其具备的属性。

![D:\111sheji\文档管理系统\wendangguanli\\img\用户.jpg](/md/blog.007.jpeg "D:\111sheji\文档管理系统\wendangguanli\\img\用户.jpg")
用户实体属性图

（3）下图是公告信息实体和其具备的属性。

![D:\111sheji\文档管理系统\wendangguanli\\img\公告信息.jpg](/md/blog.008.jpeg "D:\111sheji\文档管理系统\wendangguanli\\img\公告信息.jpg")
公告信息实体属性图

（4）下图是字典表实体和其具备的属性。

![D:\111sheji\文档管理系统\wendangguanli\\img\字典表.jpg](/md/blog.009.jpeg "D:\111sheji\文档管理系统\wendangguanli\\img\字典表.jpg")
字典表实体属性图

（5）下图是用户表实体和其具备的属性。

![D:\111sheji\文档管理系统\wendangguanli\\img\用户表.jpg](/md/blog.010.jpeg "D:\111sheji\文档管理系统\wendangguanli\\img\用户表.jpg")
用户表实体属性图

（6）下图是资料信息实体和其具备的属性。

![D:\111sheji\文档管理系统\wendangguanli\\img\资料信息.jpg](/md/blog.011.jpeg "D:\111sheji\文档管理系统\wendangguanli\\img\资料信息.jpg")
资料信息实体属性图
### 4.3.2 数据库表结构
在上述内容中，已经设计出相应的E-R模型，就可以在数据库里面根据各个实体创建相应的数据表，不过在初次使用数据库工具的时候，是需要创建一个针对程序的数据库文件，有了此步操作之后，才在刚创建的数据库文件里面创建数据表，创建数据表需要涉及到字段的设计，主键的设计，字段长度与类型的设计等内容，只有设计好的数据表结构才可以按照此规则存放对应的程序数据。这里举个例子，就拿上面提到的用户实体来说吧，用户具备的属性值，比如账号，比如联系方式与电话等都可以设计成该用户数据表里面的字段，然后对这些字段设计其数据类型，长度，并选择该表的主键作为此用户数据表的唯一标志。数据库里面的各个数据表都有它们的主键，这样也是为了方便区分各个数据表。 

表4.1配置文件表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|name|String|配置参数名称|是|
|3|value|String|配置参数值|是|
表4.2字典表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|dic\_code|String|字段|是|
|3|dic\_name|String|字段名|是|
|4|code\_index|Integer|编码|是|
|5|index\_name|String|编码名字|是|
|6|super\_id|Integer|父字段id|是|
|7|beizhu|String|备注|是|
|8|create\_time|Date|创建时间|是|
表4.3论坛表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|forum\_name|String|帖子标题|是|
|3|yonghu\_id|Integer|用户|是|
|4|users\_id|Integer|管理员|是|
|5|forum\_content|String|发布内容|是|
|6|super\_ids|Integer|父id|是|
|7|forum\_state\_types|Integer|帖子状态|是|
|8|insert\_time|Date|发帖时间|是|
|9|update\_time|Date|修改时间|是|
|10|create\_time|Date|创建时间|是|
表4.4公告信息表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|news\_name|String|公告信息标题|是|
|3|news\_types|Integer|公告信息类型|是|
|4|news\_photo|String|公告信息图片|是|
|5|insert\_time|Date|公告信息时间|是|
|6|news\_content|String|公告信息详情|是|
|7|news\_delete|Integer|假删|是|
|8|create\_time|Date|创建时间|是|
表4.5token表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|userid|Integer|用户id|是|
|3|username|String|用户名|是|
|4|tablename|String|表名|是|
|5|role|String|角色|是|
|6|token|String|密码|是|
|7|addtime|Date|新增时间|是|
|8|expiratedtime|Date|过期时间|是|
表4.6用户表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|username|String|用户名|是|
|3|password|String|密码|是|
|4|role|String|角色|是|
|5|addtime|Date|新增时间|是|
表4.7资料信息表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|wendang\_name|String|资料标题|是|
|3|wendang\_types|Integer|资料类型|是|
|4|wendang\_erji\_types|Integer|二级分类|是|
|5|wendang\_photo|String|资料封面|是|
|6|wendang\_file|String|文件|是|
|7|yonghu\_id|Integer|用户|是|
|8|wendang\_yesno\_types|Integer|审核结果|是|
|9|wendang\_content|String|资料详情|是|
|10|wendang\_delete|Integer|假删|是|
|11|create\_time|Date|创建时间|是|
表4.8用户表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|username|String|账号|是|
|3|password|String|密码|是|
|4|yonghu\_name|String|用户姓名|是|
|5|sex\_types|Integer|性别|是|
|6|yonghu\_id\_number|String|身份证号|是|
|7|yonghu\_phone|String|手机号|是|
|8|yonghu\_photo|String|照片|是|
|9|yonghu\_types|Integer|专业|是|
|10|yonghu\_delete|Integer|假删|是|
|11|create\_time|Date|创建时间|是|

# 5 系统实现
对文档管理系统进行了前面的系统分析，系统设计之后，接下来的环节就是文档管理系统的具体编码实现功能的部分。这部分内容会显示系统各个功能的具体界面运行效果。
## 5.1 管理员功能实现
### 5.1.1 用户管理
管理员可以对用户信息进行添加，修改，删除，查询操作。

![](/md/blog.012.png)

图5.1 用户管理页面
### 5.1.2 资料类型管理
管理员可以对资料类型信息进行添加，修改，删除，查询操作。

![](/md/blog.013.png)

图5.2 资料类型管理页面
### 5.1.3 公告信息管理
管理员可以对公告信息进行添加，修改，删除，查询操作。

![](/md/blog.014.png)

图5.3 公告信息管理页面
### 5.1.4 管理员管理
管理员可以对管理员信息进行添加，修改，删除，查询操作。

![](/md/blog.015.png)

图5.4 管理员信息管理页面
## 5.2 用户功能实现
### 5.2.1 资料信息添加
用户登录后可以在资料管理里面添加资料信息。

![](/md/blog.016.png)

图5.5 资料信息添加页面
### 5.2.2 资料信息管理
用户可以看到自己添加的资料信息，包含是否审核状态以及可以对自己添加的资料信息进行添加，修改，删除，查询操作。

![](/md/blog.017.png)

图5.6 资料信息管理页面

### 5.2.1 论坛管理
用户可以在论坛管理里面查和回复相关论坛信息。

![](/md/blog.018.png)

图5.7 论坛管理页面
### 5.2.2 资料信息
用户可以在首页的资料信息里面查看和下载资料信息。

![](/md/blog.019.png)

图5.8 资料信息页面

# 系统










