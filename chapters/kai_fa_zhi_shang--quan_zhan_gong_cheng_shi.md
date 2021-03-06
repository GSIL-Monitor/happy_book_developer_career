# 全栈工程师

不要指望靠流程解决问题。最终是靠人。

## 角色的缘起

受丰田的影响，软件行业中的从业人员，被人为的分成若干角色：

架构师（项目管理者）
UI设计，
程序员（码农）
测试
运维
产品经理

如果是从产品的角度来看，这些角色需要精简（一个人身兼多职）

## 沟通的成本太高

一个人做项目，可以不需要与人交流，这个人在沟通上的成本是0 。

两个人做项目，必须两个人互相交流。

根据实际情况来看，一个项目的最佳人选是4个人以下。最好是2，3个精英。因为划分任务
很负责：

- 你必须做到尽量公平：每个人的任务一样多
- 你必须做好划分的合理：每个子任务之间是可以独立拆分开的，不互相依赖的。
- 你必须考虑到项目的工期，让擅长的人做擅长的事。或者预先留出学习的时间。


## 不好的流程会催生出坏人

最常见的例子：为什么 产品经理与程序员的关系一直被人诟病？
（产品经理被打）

为什么测试人员跟开发人员是矛盾？

为什么运维人员讨厌部署？


例如，在互联网公司中，程序员的代码要生效，是需要给运维人员写申请的。过程一般是：

- 程序员填写好一份部署文档
- 程序员把部署文档 写邮件给运维人员
- 运维人员要求程序员打印出来，签字
- 运维人员按照程序员的要求，操作服务器。
- 运维人员告诉程序员：部署完毕，你快测试看有没有问题。

这里的切身体会是，程序员每做一次部署，需要：

- 写一份部署文档
- 签字，证明除了问题都是程序员的责任
- 给运维的人发邮件，打电话
- 做最简单的一个部署，也要2，3个小时。

运维人员每做一次部署，也仿佛掉了一层皮：

- 拿到部署文档
- 按照部署文档的提示，一步步的操作数据库。
- 由于程序不是运维人员写的，所以他完全不知道服务器变慢时，是哪里出的问题，如何调试
- 部署的时候会想，怎么你的python 部署过程跟java部署完全不一样？
- 出问题的时候会想，怎么你的代码出问题要我给你承担责任？

所以，出了问题的时候，大家就会互相指责：

程序人员：服务器不归我管，是运维没有及时增加服务器数量。
运维人员：代码不是我写的。是程序写的不好，测试不完备。
测试人员：代码不是我写的。我在上线前一直在加班。人肉测试达不到100%覆盖率。

## 不要把程序员分成后端和前端

对于java/ios/php这样的经典开发语言，是比较啰嗦的。java程序员无法同时掌握多种语言。
比如 CSS, javascript.

所以在十年前，招聘帖子就分成 web开发工程师和 html 前端工程师。
对于HTML前端工程师, 他的工作任务是把美工设计的静态网站图片，设计成html + CSS + javascript
代码。

这是我知道最早的前后端之说。

后来，随着移动端开发的兴起，又有很多人开始参与android/ios/winphone等的开发。
随便一款语言的学习都要读厚厚的一本书，所以做android/ios的人根本无暇学习web端
的知识。

所以，大家也就接受了这样的观点：必须分成前后端。

web中的前后端能相处的相安无事。但是web端 与 app端的开发者就不友好了。因为很多时候
会出现踢皮球的现象：

某个项目开始后，需求定好了，该划分工作了，但是发现有个需求，放在app端也可以，
放在web端也可以。该怎么办？

于是踢皮球的情况就产生了。web端认为这个东西应该做在app端，自己的任务已经够多了。
app端认为应该做在web端，这个事情可以在web端做，为什么就不做呢？

所以，这样的结果往往是：

- 前后端关系不好，各种踢皮球
- 没出问题还好。出了问题互相推诿，几次下来不踢皮球的人发现自己卖力不讨好，也开始踢了。
- 工作效率低下。半天可以做好的东西，往往按照一周来估计。
- 产品经理两面不是人。 前后端都觉得你干嘛要设计这个功能呢？


## 全栈工程师的特点

全栈工程师就可以解决这个问题。

他的特点是：

- 又能做web端程序
- 又能做app端程序
- 又能做HTML/CSS/JQUERY程序
- 还能把静态图片切图.
- 还能做自动化的测试。
- 还能参与需求，做原型图。

特点是：

出了问题不会互相指责
技术全面，又懂服务器，又懂代码，开发的质量自然就好。
解决问题速度特别快
为公司省钱。

在悦家（www.yuewz.com）和优优宝(www.uubpay.com)，我们完全采用了这样的方式：一个全栈工程师
集： 开发人员、运维人员、测试人员于一身，又会写移动端代码，又会写服务器端代码，又会部署，
极大的减轻了沟通的成本，减少了不同角色之间的纠纷，提高了效率。

我们程序员的工作内容是这样的：

项目开始时，先跟产品经理，一起把需求确定下来。参与到定制流程图。

需求定好后，自己主动申领任务。

美工做UI设计。与此同时，程序员开始工作，开两个调试窗口： app端是一个，web页面是一个。
他需要什么功能，先在app 端写一部分程序，需要接口的时候，再切换到web端的代码，
写程序，调试。然后再切换回来。。。 因为自己要什么接口自己是最清楚的，不需要沟通，
立马写好了。

在每天下班前：
程序员提交代码到web服务器，部署，重启服务器使之生效。
程序员发布最新的app代码到应用商店。或者把它按照到产品经理的手中。

产品经理每天早上，把测试机上的最新代码过一遍，看看其中有哪些BUG。 记录在
BUG系统中。然后带领程序员开早会：哪些功能已经实现了，哪些BUG已经修改完，
还差哪些任务。

这样的团队，只需要：

产品经理兼测试： 一名
全栈工程师：2~4名(这里面有一个技术小组长）
UI美工：1名

技术负责人只需要：
- 提供技术支持
- 出现技术争论时，直接拍板。
- 查看存在哪些问题。

## 实战情况

根据实际情况来看，全栈工程师完全避免了前后端踢皮球的问题，完全避免了沟通耗时的问题。
哪怕是菜鸟，都可以通过避免上述的问题而间接提高生产率。

在悦家和优优宝，一个项目，通常有2个一年经验的全栈工程师就足够了。

## 有可能产生全栈攻城狮的技术背景

一般来说, java, php,c 等传统语言背景的人,无法做成全栈攻城狮. 因为他们所使用的语言过于复杂,
笨重,很多时候他们是有心无力去学习其他知识的.

全站工程师比较多的是 ruby 等新兴语言,这类语言的特点是: 轻盈, 表达力强, 简洁.

粗略的讲: 如果一门语言不需要使用什么设计模式,就能工作的很好,那么这门语言就是比较轻盈的.
