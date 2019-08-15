# 简历

## 个人信息

祁煌，男，前端开发工程师。现就职于上海汉得研发中心，负责猪齿鱼Choerodon框架的开发和维护。

于2017年毕业于西南财经大学，本科学历，计算机科学与技术（金融信息化）专业。

## 联系方式

邮箱：

1. qihuang@ghy.cn

电话：

1. 18018514285

## 个人情况概述

已工作两年，对js有比较深入的了解，能够快速开发。

- 熟悉React（及相关库如react-router，mobx，ant-design等）能快速开发，了解react部分高级特性
- 熟悉webpack，parcel，rollup等打包工具，能够开发webpack loader和插件，熟悉webpack编译的流程和原理，能够进行配置和优化
- 熟悉babel原理，能够开发babel插件
- 能够根据需求开发脚手架项目，如@choerodon/boot
- 了解和能够开发ui组件库，如choerodon-ui
- 能够根据需求探索和制定新方案
- 熟悉敏捷开发流程
- 熟悉devops思想
- 对持续集成、持续发布（CI/CD)有所了解
- 熟悉Git flow模型，有较好的开发习惯
- 对测试有所了解

## 证书

1.英语六级

## 工作经历：

### 上海汉得信息技术股份有限公司 研发中心 2013.09~至今

&emsp;&emsp;研发中心于2018年5月开源Choerodon猪齿鱼平台。Choerodon猪齿鱼是一个开源企业服务平台，是基于Kubernetes的容器编排和管理能力，整合DevOps工具链、微服务和移动应用框架，来帮助企业实现敏捷化的应用交付和自动化的运营管理，并提供IoT、支付、数据、智能洞察、企业应用市场等业务组件，来帮助企业聚焦于业务，加速数字化转型。

&emsp;&emsp;采用容器技术和Kubernetes提供的容器编排和管理能力，将企业专有云和公有云基础设施平滑地融合在一起，使混合云平台具有了良好的扩展性和延伸性，以及在发生任何部分损坏或宕机时执行自修复的快速响应能力，确保应用系统具有提供稳定高效服务的能力。

&emsp;&emsp;以DevOps为理念，结合敏捷的软件开发实践，有效促进开发（应用程序/软件工程）、技术运营和质量保障（QA）人员之间的沟通、协作与整合；同时，持续集成与持续交付提高了公司对市场的响应速率和软件交付的质量。

&emsp;&emsp;采用Spring Cloud作为微服务架构，将系统模块拆分成多个各自独立的微服务，降低应用模块的耦合度。并且，利用容器编排和管理工具，结合DevOps最佳实践，企业对应用的一部分使用更快、更敏捷的方式进行开发、部署和更新工作，因此能够对新的市场需求和竞争状况做出更及时和更灵活。

&emsp;&emsp;主要模块包括：Devops管理，IAM管理，微服务管理，敏捷管理，测试管理，Wiki管理。

### 项目经历： 

#### Choerodon框架组开发 – 2018.1-至今

&emsp;&emsp;框架组主要负责从前端框架层面提供支持，包括项目脚手架的维护和优化，部分技术选型，规范制定，方案探索，UI库的维护和优化，新技术的甄选和推进。

工作内容：
- 开发@choerodon/boot脚手架   
通过nunjunks模板进行多模块整合打包，整合单体应用和微服务两种开发模式，提供了包括发布，编译等一系列钩子方便开发

- 设计和实现了基于npm形式的发布和依赖模块方式  
由传统的所有模块都在一个总项目下，统一编译转为各个模块编译后进行模块发布，使各团队维护自己的模块时更加简单，责任更加清晰，而且使总前端的打包时长从30分钟缩短至12分钟

- 优化原有环境变量注入方案，设计并实现了前端环境变量注入方案  
通过JS全局对象特性，使用shell脚本和node模拟合并用户自定义变量和内置变量，并且提供在镜像在部署时能够根据不同环境进行变量替换的途径，增加灵活性和便于排错，避免了原来增加变量需要框架层做出修改，不利于维护和协调的困难

- 设计并实现了前端运行时主题色替换的方案  
为了应对客户要求运行时的主题色替换，原先的less变量注入方案（只能满足编译时替换）已经不再满足。根据webpack打包流程，对输出文件前的样式文件进行处理，收集出所有相关颜色值进行单独管理，提供运行时替换的方案。

- 设计和优化了平台的权限体系和多语言体现，提供了如ws和文件服务统一处理的方式  
基于约定先行的方式，设计了权限统一收集判断然后分发处理的机制。提供了外层websocket处理，使调用websocket更加简单和符合编程方式

- Low-Code低代码平台开发  
通过高度场景化的假设和数据库关系的抽象，开发了Low-Code平台，平台包括数据库管理、模型管理、模型设计、模型发布、菜单管理、模型预览和模型反向等部分。  
主要负责数据库管理、模型管理、模型发布、菜单管理和模型反向等部分，打通整条线路，通过组件封装的思想实现模型反向展现的封装（通过结构化数据展示成具有逻辑和动作的页面），实现一对一，一对多，多对多等基础场景反向，已被公司Hzero框架集成并进行二次开发。

- 适合于choerodon平台的快速开发平台方案探索和设计  
以Fusion Design为参照，融合把设计引入整个开发流程并且起先行作用、以token来管理变量和物料化组件的独特思想，独立设计了适应于Choerodon平台的快速开发平台方案，并且对Fusion Design提供的脚手架项目进行阅读和个性化改造。

- 制定了Choerodon平台前端开发规范  
初步制定了大家都普遍接受的前端开发规范，强调lint的必须性，推行hooks和函数式开发方式，规约开发习惯，使大家的代码更规范和“相似”，解决“优化代码不如自己重写，各有各的习惯”的交流问题。

- 日常choerodon平台维护和开发  
包括但不限于菜单管理，组织管理，项目管理，全局管理（多层级），用户管理，角色管理等企业级场景化的日常开发和维护。

#### Choerodon敏捷开发组 – 2018.4-2018.9

&emsp;&emsp;敏捷开发组是Choerodon平台敏捷思维的一个体现，可以简单地概括为线上看板和配套平台，参考和汲取了Jira，ones等团队协作开发流程，主要包括故事地图，待办事项，活跃冲刺，问题管理和统计报告等几个主要部分，其中故事地图是用于迭代开始前的规划和初步排板的，待办事项是进行冲刺的任务和子任务的拆分，故事和故障的建立和管理的场所，活跃冲刺是当前冲刺所有任务进度的直观反馈，统计报告从各个不同的维度（燃尽图，经办人分布，史诗分布，版本分布，迭代速度等）来对迭代有个更直观地展示，帮助更好地规划和交付。

工作内容：

- 使用React实现敏捷相关页面（故事管理，故事地图，报表，系统设置，模块管理）  
使用Choerodon-ui为组件库，以mobx作为状态管理库进行复杂业务场景的开发，包括列表展示，表单提交，富文本编辑器，附件上传，拖拽等多种前端场景。在一个月的时间内完成快速交付，经过不停迭代后成为Choerodon平台体现敏捷思想的主要载体。

- 实现故事管理接收多页面参数并高可查询化设计  
- 对项目进行性能优化，尤其是优化故事地图布局，提高组件渲染性能，整理拖拽情况，使页面可用性提升  
通过更细粒度的组建拆分，PureComponent和shouldComponentUpdate的使用，逻辑和呈现，懒显示的分离和场景的抽离优化，使得原本在200张卡片就会比较卡顿和占用超大内存的情况得到解决，使用流畅且内存占用合理。

#### HAP（4.0）框架升级 – 2018.9至2019.3

&emsp;&emsp;汉得应用开发平台（HAND Application Platform）是汉得公司为了应对移动互联网化、应用云端化、海量数据化和数字化服务转型的应用开发平台，是中台化产品和应用开发的基础平台。HAP采用开源的Java EE技术体系，平台设计灵活可扩展、可移植、可应对高并发需求。

&emsp;&emsp;传统企业开发的过程中，客户往往需要对不同的技术框架进行选型研究，各种不同技术平台的版本不一致以及框架的兼容性问题常常耗费大量的研究时间。

&emsp;&emsp;HAP平台基于Java EE开源技术体系构建，支持多种主流数据库，可以很容易的部署在包括公有云或私有云在内的各种 PaaS平台，支持在Docker等虚拟化容器中部署，提供了从前端到后端的一站式技术解决方案。客户无需再为各种技术选型而耗费大量宝贵时间，节省出更多精力来专注业务实现,快速应对需求变化。

&emsp;&emsp;随着前端技术的快速发展，HAP框架也由原来的Jquery向React进行升级，升级过程中对原先页面仍提供支持，达到逐步迭代升级的目的。

工作内容：

- 动态模块加载探索，高度场景化的表格和表单组件调研和探索  
在绝大部分企业级应用中，表格和表单都是具有场景化的，以表格展示，表单修改、添加为展现方式，在表格上有多种操作，所以提取出公用的逻辑，以定义数据形式的方式来组织组件

- 开发choerodon-front-hap-boot作为新版HAP4.0的启动器，达成单模块和多模块的开发和发布  
为了优化目录结构、简化开发和方便版本的管理，将启动器抽出为boot npm包发布并持续迭代至今。提供了启动器，HAP前端原有页面的兼容，新页面（react）的支持，通用部分如tab页，菜单和用户管理，首选项设置等角色。其中tab页组件在react-router的基础上进行扩展实现页面缓存的功能（最后迁移至开源库react-route-cache-route）

- 为了便于后端人员开发，设计和简化两版模式模板，并规范了目录结构，调用方式等

- 组件开发  
改造和封装了Modal（弹窗，包括抽屉和confirm类型），校对并修改了绝大部分组件的样式。开发了树形组件，同时接受dataSet和原数据形式两种数据形式。修复部分组件库的问题。

#### HAP Cloud 移动端研发项目 – 2017.9至2018.1

&emsp;&emsp;该项目验证React Native为开发语言，进行移动端的微服务探索，通过CI生成镜像包，制定更新规则进行在线更新。通过提供安卓和iOS双平台的“壳子应用”，由壳子应用提供一些基本逻辑（如登录，角色验证）处理，通过本地存储的本地版本模板信息与远端的进行对比，实现模块的独立更新和管理。

主要包括：
- 安卓、iOS原生盒子应用的开发
- React Native的主应用开发
- React Native的各模块开发（数据统模块，各种基础功能的验证模块，包括地图、相机、通讯录等）

工作内容：

- 查找并解决日常开发中遇到的问题  
当时React Native为0.46+版本，部分问题和解决方案还不是非常完善，通过探索完成了chunk的打包处理和本地文件的模块对比进行处理。还在React Native中文官网进行部分翻译纠错。

- 探究并实现了RN端与原生端的信息通信，和互相调用打开关闭，实现完整的移动端外壳应用。

- 学习并实现了Swift端外壳应用，采用drawer布局，支持一个常驻的RN chunk，即主菜单界面，根据主菜单界面的操作和事件调用原生端的事件，完成模块的下载，更新。

- 封装了多个独立模块  
如调用原生的权限模块（摄像头，短信，地图权限），UI模块（按钮，条状信息栏，选择框），功能模块（图表展示监控信息模块monitor）等，基本调通开发中可能遇到的问题。
