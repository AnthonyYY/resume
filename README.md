 个人简历
 ===============
 ##个人信息
 ---------------
 **姓名**： 叶家洪
 
 **性别**： 男
 
 **毕业学校**：**福建省华侨大学** 工业设计数字工程动画专业
 ## 自我介绍

 ## 技术能力
 
 ## 项目经历
 
 ### [赛事报表 赛事数据html2PDF报告生成程序](http://123.59.46.69:3000/preview/CD93704A-793E-47B7-99BC-723886986175)
 项目地址: <http://123.59.46.69:3000/preview/CD93704A-793E-47B7-99BC-723886986175>
 实现的技术：
 * node.js
 * Express.js 提供文件的下载、访问、渲染接口
 * phantom.js 真正绘制pdf文件的模块(phantom-node)
 * heatmap.js 球员跑动热区绘制插件
 * canvas 略微复杂图形的绘制工具
 * async.js(parallel) 使用request整合后端api完成后与模板渲染数据之间的一个承轴
 * artTemplate(aui) 作为node.js的模板引擎 最后将所有页面模块 include 到一个main文件
 >phantom.js这个第三方木块渲染不了异步获取的东西，不适合使用前后端分离的方案，放弃使用angular，
 java渲染freemarker方案需要后端同学的介入 构建的开发环境也不够友好pass
 最后考虑以node.js作为中间层整合后端提供的api 拿到数据 用artTemplate这个模板引擎渲染数据，
 模板引擎难以绘制的复杂图形，将需要的数据以json字符串的形式提供给client端在client端执行canvas脚本绘制出来，
 整个pdf文件中的球场，球员，足球，方向箭头都是用canvas 绘制出来的
 node.js 提供一个地址端口作为开发环境显示pdf文件的html版本的预览模式，用于调试布局，
 另外提供一个调用pdf文件的渲染查看的接口和pdf文件下载的接口给其他网站使用，
 按照以上思路我实现了整个项目的开发环境的构建供其他前端开发者实现页面布局，
 中间也参与实现了页面的layout工作 canvas 的绘制工作，后期项目在centos的部署工作,
 这个项目的完成使我对node.js有了更深入的了解和运用 并且对于node.js 作为中间层的使用有了更深的理解，
 这也是我第一个在公司部署上线被使用的node程序，
 开发遇到的问题： 之前对只专注在代码对业务逻辑的处理，忽视了性能方面的考量，
 程序处理过程中没有对各种情况下的程序处理结果后正确关闭调用的进程导致在使用过程中曾导致服务器崩溃，后面在代码做了处理解决了问题
 
 
 ## 自我简介(精简版)
 
 ## 自我简介(聒噪版)
 
 大四下学期开始接触web并投入学习 在校期间玩转了一段时间的CSS3习了点jQuery就觉得“学有所成”便出去面试实习岗位并在厦门蓝尚信息科技(<http://www.ulandian.com/>)
 工作了三个月期间负责公司官网的搭建和维护同时完成宣传招聘微信html5页面的制作。至此还未与后端交互的经验。毕业后来到简极科技担任前端开发工程师一职
 
