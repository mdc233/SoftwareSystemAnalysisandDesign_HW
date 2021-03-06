* 用例的概念

答:<br>
用例是代表系统中各项目相关人员之间就系统的行为所达成的契约，用例描述了在不同的条件下，系统对某一项目相关的人员的请求所作出的响应。<br>


* 用例和场景的关系？什么是主场景或 happy path？

答：<br>
根据执行者做出的请求和请求涉及的条件，系统将执行不同的行为序列，每一个行为序列称为一个场景，一个用例是多个不同场景的集合。<br>
happy path是指一个在执行过程中没有任何异常和错误的场景，例如，验证信用卡号的功能的happy path就是没有任何验证规则引发错误的场景，从而能让执行成功地继续到最后，最后得到肯定的响应。<br>
主成功场景是指，在一个该场景中，主执行者完成了目标，所有项目相关的人员的利益得到了满足。<br>

* 用例有哪些形式？

答：<br>
文本形式。有brief、Casual、Fully三种格式。

* 对于复杂业务，为什么编制完整用例非常难？

答:<br>
编写用例中对系统目标的描述需要项目开发组、项目管理人员、用户代表等多方的参与，需要他们对项目的费用和复杂性进行讨论，协商开发哪些功能，讨论如何组建开发小组。<br>
编写用例中对异常情况处理的描述需要用例编写者集中讨论主成功场景下所有可能发生的异常情况，而这一点非常难做到，需要业务专家的参与来解决。如果错误在程序员编写时才发现，此时业务专家通常已经走了，这是只能靠程序员自己的想法来编写代码，而不是努力去寻求更合理、理想的解决方法。<br>
而且完整用例格式下，用例说明文档将会非常地长。<br>


* 什么是用例图？

答:<br>
用例图是对系统环境的图像化描述，展现了系统的边界范围、什么在范围内和不在范围内以及该系统如何被使用，总结了参与者和系统的行为。<br>

* 用例图的基本符号与元素？

答：<br>
参与者，一般用小人符号表示。<br>
系统边界，一般用空心的方框表示。<br>
用例，一般用椭圆表示。<br>
关系，一般用不同类型的线条表示。<br>

* 用例图的画法与步骤

答:<br>
1. 选择系统边界<br>
2. 找到所有主执行者<br>
3. 定义每个主执行者的目标<br>
4. 编写符合用户目标的用例，用目标来命名用例<br>
5. 对用例分析是否存在扩展<br>
6. 根据上述信息按用例图标准来绘制成图。


* 用例图给利益相关人与开发者的价值有哪些？

答:<br>
合理的用例识别（制作的用例图），通常给团队带来以下利益：<br>
 1. 明确系统的业务范围、服务对象（角色）、外部系统与设备<br>
 2. 帮助识别技术风险，提前实施关键技术原型公关与学习<br>
 3. 易于评估项目工作量，合理规划迭代周期，规划人力需要<br>




* 选择2-3个你熟悉的类似业务的在线服务系统（或移动 APP），如定旅馆（携程、去哪儿等）、定电影票、背单词APP等，分别绘制它们用例图。并满足以下要求：
  * 请使用用户的视角，描述用户目标或系统提供的服务
  * 粒度达到子用例级别，并用 include 和 exclude 关联它们
  * 请用色彩标注出你认为创新（区别于竞争对手的）用例或子用例
  * 尽可能识别外部系统和服务

![image1](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/HW4%E7%BE%8E%E5%9B%A2.png)
![image1](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/HW4%E9%A5%BF%E4%BA%86%E4%B9%88.png)
  
* 然后，回答下列问题：
  * 为什么相似系统的用例图是相似的？
  * 如果是定旅馆业务，请对比 Asg_RH 用例图，简述如何利用不同时代、不同地区产品的用例图，展现、突出创新业务和技术
  * 如何利用用例图定位创新思路（业务创新、或技术创新、或商业模式创新）在系统中的作用
  * 请使用 SCRUM 方法，选择一个用例图，编制某定旅馆开发的需求（backlog）开发计划表
  * 根据任务4，参考 使用用例点估算软件成本，给出项目用例点的估算


1. <br>
答: 因为相似系统的用户群体高度重合，用户的需求也基本是一样的，为了满足一样的需求相似系统提供的服务也大多类似，因此用例图也相似。另一方面，系统的功能开发也存在相互借鉴相同类型的成熟应用功能的现象。<br>

2. <br>
答：不是定旅馆业务<br>

3. <br>
答：那上图的美团和饿了么做例子，在用例图中将创新功能用颜色标出，再比较这两个相似系统，于是便一眼看出两个系统的创新点是什么，在整个系统处于什么层次地位。<br>

4. <br>
答：首先选择一个用例图:<br>

![image](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/%E5%AE%9A%E6%97%85%E9%A6%86%E7%94%A8%E4%BE%8B%E5%9B%BE.png)


编写backlog:<br>
Imp: 重要性,产品负责人评出一个数值，指示这个故事有多重要。例如10或150.分数越高约重要。<br>
est：初始估算，团队的初步估算，表示与其他故事相比，完成该故事所需的工作量。最小的单位是故事点(storypoint)，一般大致相当于一个man-day(人天数)，例如把3个人关在一起，大约需要4天时间，那么初始估算的结果就是12个故事点。<br>


![image](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/%E5%AE%9A%E6%97%85%E9%A6%86backlog.png)

5. <br>
用例点估算成本的流程如下:<br>

![image](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/%E7%94%A8%E4%BE%8B%E7%82%B9%E6%96%B9%E6%B3%95%E6%B5%81%E7%A8%8B.jpg)

根据流程:<br>
1. 计算Size = UUCP * TCF; UUCP = AW + UCW. 依据：<br>

![image](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/AW.png)
![image](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/UCW.png)
![image](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/TCF.png)


因此，TCF = 0.28+0.6 ，UUCP = 8+120+40， Size = 168*0.88 = 147.84<br>

2. 同理，依据：<br>

![image](https://github.com/mdc233/SoftwareSystemAnalysisandDesign_HW/blob/master/EF.png)

可知， EF = 1.4 - 0.03*23 = 0.71. <br>

3. 由于条件不足，无视H和SE， Effect = Size * EF = 147.84 * 0.71 = 105
