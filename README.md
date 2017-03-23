个人简历
===============
基本信息
---------------
**姓名**： 叶家洪

**性别**： 男

**毕业学校**：**福建省华侨大学**  工业设计数字工程动画专业

> "Anything that can be written in JavaScript will eventually be written  in JavaScript!" 你打我呀

## 技术能力
* 掌握的javascript类库：jquery、jqueryUI、zepto
* 掌握的javascript框架：Angular.js、bootstrap
* 掌握的css预处器：less
* 掌握的项目构建工具与模块打包工具：gulp、webpack
* 掌握的测试框架及工具：karma、mocha
* 掌握基本的后端开发：node.js、mongodb、redis、socketio、express.js
* 掌握一些桌面端的开发手段：nw.js
* 掌握的开发版本管理调试工具：sublime、webstorm、intelliJ IDEA、atom、git、chrome 调试工具、npm、bower、yarn
* 了解过 vue.js、react.js、meteor.js、typescript、Electron.js、docker



## 项目经历

### [GSM-足球赛事组织报名管理系统](http://gsm-test.xiaojiang.me/gsm)
访问地址: http://gsm-test.xiaojiang.me/gsm

###### 实现技术手段:

* jquery
* jquery-ui
* require.js
* angular.js
* ui-bootstrap
* flat-ui

###### 项目简介

这是一个足球赛事管理系统 对于赛事报名方(登陆账号)而言是个赛事报名跟踪系统 对于赛事组织方(登陆账号)而言是个赛事组织管理系统
该系统早期技术选型出于对ie6,ie7 的考量第一个大版本部分使用后端渲染freemarker模板的方案实现的，
前端主要通过jQuery jQuery-UI 和其他基于jQuery的插件实现前端用户交互逻辑和一些数据的异步请求加载，
该版本的样式层直接使用的css，更没有gulp，grunt之类的构建工具的接入。
后来的第二个大版本直接完全重构，纯粹的前后端分离，前端使用angular-ui-router实现路由功能，
在flat-ui 和 ui-bootstrap 的基础上实现页面的样式及交互功能
前端通过和后台提供的restful api实现交互数据 完成增删改查显示等诸多操作
相比于使用jQuery 对使用原生javascript 带来的生产力解放，angular操作数据的方式也让jquery操作DOM的方式看起来如同是刀耕火种。
当然angular也有很多不适用的场景 ng1 在seo方面的薄弱和双向数据绑定带来的性能问题也是不容忽视的。
(14299999999 admin)

### [校园足球球员苗子库](http://gsm.xiaojiang.me/Seeding)
访问地址：http://gsm.xiaojiang.me/Seeding (admin admin123)
###### 实现技术手段
- angular
- ui-bootstrap
- ng-highchart
- flat-ui

###### 项目简介

这个系统是用作校园足球员人才苗子库的数据管理系统. 
该系统包括两大部分，球员筛选页面和球员详情页面(球员简历、球员战绩、球员对比三个tag)
基于flat-ui风格的样式



### [赛事报表 赛事数据html2PDF报告生成程序](http://123.59.46.69:3000/preview/CD93704A-793E-47B7-99BC-723886986175)
项目地址: <http://123.59.46.69:3000/preview/CD93704A-793E-47B7-99BC-723886986175>
###### 实现技术手段
* node.js
* Express.js 提供文件的下载、访问、渲染接口
* phantom.js 真正绘制pdf文件的模块(phantom-node)
* heatmap.js 球员跑动热区绘制插件
* canvas 略微复杂图形的绘制工具
* async.js(parallel) 使用request整合后端api完成后与模板渲染数据之间的一个承轴
* artTemplate(aui) 作为node.js的模板引擎 最后将所有页面模块 include 到一个main文件

###### 项目简介
phantom.js这个第三方模块渲染不了异步获取的东西，不适合使用前后端分离的方案，放弃使用angular，
java渲染freemarker方案需要后端同学的介入 构建的开发环境也不够友好pass
最后考虑以node.js作为中间层整合后端提供的api 拿到数据 用artTemplate这个模板引擎渲染数据，
模板引擎难以绘制的复杂图形，将需要的数据以json字符串的形式提供给client端在client端执行canvas脚本绘制出来，
整个pdf文件中的球场，球员，足球，方向箭头都是用canvas 绘制出来的，
为了提高开发效率也在node程序里加入了gulp的工作流
node.js 提供一个地址端口作为开发环境显示pdf文件的html版本的预览模式，用于调试布局，
另外提供一个调用pdf文件的渲染查看的接口和pdf文件下载的接口给其他网站使用，
按照这些思路我整合以上技术我实现了整个项目的开发环境的开荒工作构建了基础开发环境供其他前端开发者实现页面布局，
中间也参与实现了页面的layout工作 canvas 的绘制工作，后期项目在centos的部署工作。
最后项目也以快于预期的时间完成工作并且开发过程相对友好减轻了开发压力
这个项目的完成使我对node.js有了更深入的了解和运用 并且对于node.js 作为中间层的使用有了更深的理解，
这也是我第一个在公司部署上线被使用的node程序，
开发遇到的问题： 之前对只专注在代码对业务逻辑的处理，忽视了性能方面的考量，
程序处理过程中没有对各种情况下的程序处理结果后正确关闭调用的进程导致在使用过程中曾导致服务器崩溃，后面在代码做了处理解决了问题

### [专利管理系统软件](http://pan.baidu.com/share/link?shareid=102749&uk=)
下载地址： <http://pan.baidu.com/share/link?shareid=102749&uk=>
###### 实现技术手段
* nw.js(node.js + chromium) 软件开发的技术平台
* angular.js 协助实现数据可视化的框架
* linvodb3 用于实现专利数据存储与查询的数据库
* ng-highchart 用于专利统计图表显示的第三方模块
* node-xlsx 解析excel 表格以来的模块
* md5 登陆模块实现的主要依赖
* blue-bird 项目promise化
* NSIS window exe程序打包工具

###### 项目简介
这是一个可以安装在window系统运行的(理论上在mac OS和liniux上也是可以安装运行的)的专利查询系统的exe文件，
考虑到无法对winXP系统的兼容当时并未选择更倾向的Electron.js主要框架，而是选择了 nw.js
程序的主要功能就是导入excel表格文件 读取文件的专利数据信息保存到数据库 并且提供专利项的查询展示统计等功能，
程序通过md5实现伪登陆功能，登陆的实现不需要与数据库交互，只要用户名和密码的组合通过结合md5的加密算法就可以登陆
excel表格的数据内容并不复杂 因此一个轻量级的非关系型数据库就可以胜任
考虑到程序的体积大小和移植性当时弃用了MongoDB,
也没有选择轻量级的关系型数据库sqlite3，
最后选用了linvodb3 这个数据库(https://github.com/Ivshti/linvodb3)
Gituhb文档首页这样描述该数据库Persistent database for Node.js/NW.js/Electron with MongoDB/Mongoose-like features and interface on top of LevelUp
然后使用node.js 的文件系统配合input[type='file']实现了程序专利图片和专利pdf文件的批量导入功能(导入到程序中)
通过ng-highchart 实现多项专利的统计功能
通过linvodb3实现程序的专利搜索
这个项目的实现对我而言在数据库上的设计上比较不完善，数据库只保存了excel文件导入的所有信息，其余的所有信息都是在query的时候计算出来的，
比如每一次程序打开时程序的导航栏的标题数据都遍历了所有专利项，从所有专利项的标题属性中distinguish出所有不同项的集合作为导航栏的标题，
后来想想是可以在数据导入完成后将这个计算结果持久化在数据库供查询使用的，毕竟客户端的数据库没有网络请求过程的
这个项目完全是个人外包项目

### [茵战-足球赛事赛况直播网站](http://106.75.60.196:8080/wap)
访问地址(**手机访问**)：http://106.75.60.196:8080/wap

###### 实现技术手段
* angular.js
* video.js
###### 项目简介
这是个手机端足球赛事直播网，
选择特定联赛后可以显示联赛的各种数据，积分，排行，榜单，球队数据，球员数据，
可以实现赛事直播，录播，集锦回放，实况文字直播，比赛数据统计显示等功能

### [](http://106.75.60.196:8080/Seeding)

### [公司官网开发与维护](http://www.gengee.com/)
访问地址: http://www.gengee.com/

###### 实现技术手段:
* bootstrap
* jQuery
###### 项目简介

公司官网早期的开发与维护工作

## 自我简介

###### 经历简介
大四学期开始接触web前端 一路自学 在校期间曾在蓝尚信息科技(<http://www.ulandian.com/>)实习三个月，负责公司官网的搭建维护和微信html5页面的制作。
2015年6月份毕业7月入职简极科技担任前端开发工程师职位至今。在职期间在多个项目担任重要角色，项目的评审、开荒构建、前端工作流工程化、主要开发职责。
任职过公司前端开发组长带过人(公司早期前端团队很小、巅峰时期4人规模)。连续两年在公司的绩效评定为A。
2016年开始至年终在公司git仓库的代码commit次数排名第一，代码总量排名第三(公司的技术团队里有共37名coder)。
在公司内部技术分享会上分享过angular的使用和测试框架karma配合mocha的使用。
###### 自我评价
我觉得自己对web技术就像对女朋友一样是真爱。但是路漫漫我的水平还需要很多历练。
我觉得自己的自学能力还不错。从业至今一路自学过来，但是很遗憾之前比较少总结自己的学习成果
我对自己的英语阅读水平比较自信 得益于此我不仅能无障碍阅读英文文档并且在stackovwerflow、github和google上得到很多帮助
我觉得自己还需要多多阅读源码

## 联系方式
邮箱1：yjh2332@gmail.com
邮箱2：yjh2332@163.com
zhihu：https://www.zhihu.com/people/xie-jia-hong-20



