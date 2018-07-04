# MarkDown 
>Markdown是一种轻量级且易于使用的语法，用于在GitHub平台上设置所有形式的书写样式。
> 
## 我们可以学到什么呢？
* Markdown格式如何使样式化协作编辑变得容易
* Markdown与传统的格式化方法有何不同
* 如何使用Markdown来格式化文本
* 如何利用GitHub的自动Markdown渲染
* 如何应用GitHub独特的Markdown扩展
## 什么是MarkDown呢？
>Markdown是在web上设计文本样式的一种方法，用来控制文档的显示;我们可以使用Markdown将文字格式化为粗体或斜体，添加图像和创建列表。大多数情况下，Markdown只是带有一些非字母字符的常规文本，比如`#`或`*`。
## 例子
### 文本  
#### 标题  
```markdown
	#		一级标题
	##		二级标题
	###		三级标题
	...
	######          六级标题
```  
#### 强调
```markdown
	This text will be italic	正常文字
	*This text will be italic*	效果为倾斜	
	_This will also be italic_	效果为倾斜

	**This text will be bold**	效果为加粗
	__This will also be bold__	效果为加粗

	_You **can** combine them_	双重叠加
```
#### 列表
##### 无序列表
```markdown
* Item 1
* Item 2
  * Item 2a
  * Item 2b
```
效果如下：  
* Item 1
* Item 2
  * Item 2a
  * Item 2b
##### 有序列表
```markdown
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
```
效果如下：  
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
#### 图片
>显示图片语法格式为`![任意文字](href)`  
```markdown
![local access image](a.jpg)	//访问本地图片，相对于当前项目的地址
![remote access image](https://www.baidu.com/img/bd_logo1.png?where=super)  //访问远程图片，是指互联网上的其他图片的地址
```
#### 链接
>语法格式为`[任意文字](herf)`
>```markdown
>百度了解一下->[百度](https://www.baidu.com)
>```
#### 引用
>使用一个`>`符号就好，例子如下
```markdown
>巫师3了解一下啦（ps:真的很棒的游戏）
```
#### 内联代码
>语法格式为
```markdown
`任意文字`
```
> 
效果如下：  
`巫师3` `角色扮演` `剧情`
