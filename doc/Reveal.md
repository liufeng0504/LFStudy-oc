# Reveal
[Reveal官网](http://revealapp.com)

Reveal是一个iOS程序界面调试工具。使用Reveal，我们可以在iOS开发时动态地查看和修改应用程序的界面。


## Reveal简介
Reveal是一个界面调试工具。使用Reveal，我们可以在iOS开发时动态地查看和修改应用程序的界面。它类似Chrome的“审查元素”功能，我们不但可以在运 行时看到iOS程序的界面层级关系，还可以实时地修改程序界面，不用重新运行程序就可以看到修改之后的效果。


2. 中间部分是一个可视化的查看区域，用户可以在这里切换2D和3D的查看方式，这里看到的也是程序运行的实时界面。

Reveal工具适合调试非Interface Builder创建的界面，Interface Builder中创建的xib和storyboard在企业开发中并不是总能胜任。




## Reveal的使用

### 用Reveal连接模拟器调试
Reveal官方介绍了好几种办法使Reveal连接模拟器，都需要修改工程文件。但如果修改了工程文件，就需要参与项目开发的所有人都装有Reveal，这其实是相当不友好的。本节要介绍一种不修改任何工程文件的办法，在实际使用中，这种办法最简单方便。该方法的步骤如下:

1. 打开Terminal，输入vim ~/.lldbinit创建一个名为.lldbinit的文件，然后将如下内容输入到该文件中:

	```
	command alias reveal_load_sim expr (void*)dlopen("/Applications/Reveal.app/Contents/SharedSu")
	```
2. 


### 用Reveal连接真机调试

### 用Reveal调试其他应用界面

### 总结