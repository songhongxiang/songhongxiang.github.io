# songhongxiang.github.io
&ensp;&ensp;&ensp;&ensp;本项目旨在建立一个完整的机器人学学习体系！
# 使用教程
## 1. 安装R语言和mindr功能包
#### Install R Language
&ensp;&ensp;&ensp;&ensp;R语言安装省略
#### Install mindr package
> [mindr](https://github.com/pzhaonet/mindr)由[pzhaonet](https://github.com/pzhaonet)开发，首先要感谢大佬提供的mindr包，让我们轻松将（.md，.Rmd）转换为思维导图！

```R
# stable version:
install.packages("mindr")
# or development version:
devtools::install_github("pzhaonet/mindr")
```
## 2. 项目参与
#### Step1：git工作空间
#### Step2：编辑`eatRobotics.md`并提交更新
#### Step3：使用[**mindr**](https://github.com/pzhaonet/mindr)将`eatRobotics.md`转换为`index.html`
---

转换教程如下：
```R
library('mindr')    #导入mindr库
getwd()             #获取当前工作目录
setwd("G:/桌面")    #设置[G:\桌面]为工作目录，此处为示例，具体目录请改为git项目目录
input<-c("test.md") #读入Markdown文档
print(input)        #打印文档目录，查看是否读入成功，如果为空字符串则失败
mm(from=input,type="file",root="mindr") #将md文件转为网页脑图
```
打开生成的`index.html`，通过网址栏确定文件生成目录，以便更新云端`index.html`

---
#### Step4：使用生成的`index.html`内容更新云端库中的`index.html`，该文件即为网页版脑图描述文件！
#### Step5：访问`songhongxiang.github.io`测试更新是否成功！


> 坦白讲，没想到有一天我会开始写R！正如古月所讲：怕什么真理无穷,进一寸有一寸的欢喜！
> 学习机器人，不仅要有理论的学习，更要重在实践，也这是我的成长秘籍！大家一起加油，撑起我们的机器人事业！

&ensp;&ensp;[**读万卷书，
也要行万里路！**](https://blog.csdn.net/weixin_43455581)
