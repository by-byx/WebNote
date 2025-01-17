![img](https://i.loli.net/2020/12/01/uXGNF6CHE9dpVQt.jpg)

```
该笔记由【不言谢】，重新整理发布。以供更好的学习交流。
笔记中的图片全部传入PicGo中，换端不会再影响阅读。
```

联系方式：

​	不言谢的网络学习日志： https://www.cnblogs.com/byx1024/

​	不言谢の日常：https://www.byx1024.top/

------



> 第01阶段.前端基础.表格

# HTML 第二天目标

 能够利用表格、列表和表单完成注册页面的综合案例

* 能出说表格用来做什么的
* 能说出列表用来做什么的
* 能说出表单用来做什么的

为了让我们页面显示的更加整齐，我们需要学习三个表（表格、表单、列表）

![guifan](https://i.loli.net/2020/12/01/Ut5szJjAFxRWr27.png)

# 表格 table(会使用)

目标：

* 理解：
  - 能说出表格用来做什么的
  - 表格的基本结构组成
* 应用：
  - 能够熟练写出n行n列的表格
  - 能简单的合并单元格
    ​

![ttt](https://i.loli.net/2020/12/01/saIKFCl7vpfg9M3.png)



**表格作用：**

存在即是合理的。  表格的现在还是较为常用的一种标签，但不是用来布局，**常见显示、展示表格式数据。**

因为它可以让数据显示的非常的规整，可读性非常好。

**特别是后台展示数据的时候表格运用是否熟练就显得很重要**，一个清爽简约的表格能够把繁杂的数据表现得很有条理，虽然 div 布局也可以做到，但是总没有表格来得方便。

![table](https://i.loli.net/2020/12/01/bB8qV7XYeLDjc1I.png)

ps:  这些地方用表格，你会觉得生活还是那么美好。。。。忍不住想说  PPAP i hava a pen  

## 1. 创建表格

在HTML网页中，要想创建表格，就需要使用表格相关的标签。

**创建表格的基本语法：**

```html
<table>
  <tr>
    <td>单元格内的文字</td>
    ...
  </tr>
  ...
</table>
```

要深刻体会表格、行、单元格他们的构成。

在上面的语法中包含基本的三对HTML标签，分别为 table、tr、td，他们是创建表格的基本标签，缺一不可，下面对他们进行具体地解释

1. table用于定义一个表格标签。

2. tr标签 用于定义表格中的行，必须嵌套在 table标签中。

3. td 用于定义表格中的单元格，必须嵌套在&lt;tr>&lt;/tr>标签中。

4. 字母 td 指表格数据（table data），即数据单元格的内容，现在我们明白，表格最合适的地方就是用来存储数据的。

   

![07table基本结构](https://i.loli.net/2020/12/01/yAzajmipMTKrl93.jpg)

**总结：**

* 表格的主要目的是用来显示特殊数据的
* 一个完整的表格有表格标签（table），行标签（tr），单元格标签（td）组成，没有列的标签

- &lt;tr>&lt;/tr>中只能嵌套&lt;td>&lt;/td> 类的单元格
- &lt;td>&lt;/td>标签，他就像一个容器，可以容纳所有的元素

## 2. 表格属性

表格有部分属性我们不常用，这里重点记住 cellspacing 、 cellpadding。

![tt](https://i.loli.net/2020/12/01/xtHXbkD7CoOeNrj.png)

我们经常有个说法，是三参为0，  平时开发的我们这三个参数    border  cellpadding  cellspacing  为  0

![07table表格属性](https://i.loli.net/2020/12/01/vWoR7ghpBudCLOV.png)

**案例1：**

![img](https://i.loli.net/2020/12/01/PNJ2t1GfYRuyO4a.png)

```html
<table width="500" height="300" border="1" cellpadding="20" cellspacing="0" align="center">
   <tr>  <th>姓名</th>   <th>性别</th> <th>年龄</th>  </tr>
   <tr>  <td>刘德华</td> <td>男</td> <td>55</td>  </tr>
   <tr>  <td>郭富城</td> <td>男</td> <td>52</td>  </tr>
   <tr>  <td>张学友</td> <td>男</td> <td>58</td>  </tr>
   <tr>  <td>黎明</td>   <td>男</td> <td>18</td>  </tr>
   <tr>  <td>刘晓庆</td> <td>女</td> <td>63</td>  </tr>
</table>
```

## 3. 表头单元格标签th

- 作用：
  - 一般表头单元格位于表格的第一行或第一列，并且文本加粗居中
- 语法：
  - 只需用表头标签&lt;th&gt;</th&gt;替代相应的单元格标签&lt;td&gt;</td&gt;即可。 

 ![th](https://i.loli.net/2020/12/01/mEjoIVfr8b1p2Cw.png)

**案例2：**

​	效果图

![tht](https://i.loli.net/2020/12/01/h7OAbFQRsPrwIzB.png)

​	代码：

***

```html
<table width="500" border="1" align="center" cellspacing="0" cellpadding="0">
		<tr>  
			<th>姓名</th> 
			<th>性别</th>
			<th>电话</th>
		</tr>
		<tr>
			<td>小王</td>
			<td>女</td>
			<td>110</td>
		</tr>
		<tr>
			<td>小明</td>
			<td>男</td>
			<td>120</td>
		</tr>	
	</table>
```

**pink老师 一句话说出他们:**

> th 也是一个单元格   只不过和普通的 td单元格不一样，它会让自己里面的文字居中且加粗

## 4. 表格标题caption

**定义和用法**

```html
<table>
   <caption>我是表格标题</caption>
</table>
```

**注意：**

1. caption 元素定义**表格标题**，通常这个标题会被居中且显示于表格之上。
2. caption 标签必须紧随 table 标签之后。
3. 这个标签只存在 表格里面才有意义。你是风儿我是沙

**案例3：**

根据要求完成以下案例：

![pa](https://i.loli.net/2020/12/01/RAwp6rY9zyxDkXa.png)



## 5. 合并单元格(难点)

合并单元格是我们比较常用的一个操作，但是不会合并的很复杂。

![he](https://i.loli.net/2020/12/01/VGAwhJzS7CtTamu.jpg)

###  5.1 合并单元格2种方式

* 跨行合并：rowspan="合并单元格的个数"      
* 跨列合并：colspan="合并单元格的个数"

![08table合并单元格](https://i.loli.net/2020/12/01/8PQ9bWumLXra4G7.jpg)

### 5.2 合并单元格顺序

> 合并的顺序我们按照   先上 后下     先左  后右 的顺序

跟我们以前学习汉字的书写顺序完全一致。

### 5.3 合并单元格三步曲

1. 先确定是跨行还是跨列合并
2. 根据 先上 后下   先左  后右的原则找到目标单元格    然后写上 合并方式 还有 要合并的单元格数量  比如 ： &lt;td colspan="3">   &lt;/td>
3. 删除多余的单元格 单元格      

## 6. 总结表格

| 标签名                    | 定义           | 说明                                         |
| ------------------------- | :------------- | :------------------------------------------- |
| &lt;table>&lt;/table>     | 表格标签       | 就是一个四方的盒子                           |
| &lt;tr>&lt;/tr>           | 表格行标签     | 行标签要再table标签内部才有意义              |
| &lt;td>&lt;/td>           | 单元格标签     | 单元格标签是个容器级元素，可以放任何东西     |
| &lt;th>&lt;/th>           | 表头单元格标签 | 它还是一个单元格，但是里面的文字会居中且加粗 |
| &lt;caption>&lt;/caption> | 表格标题标签   | 表格的标题，跟着表格一起走，和表格居中对齐   |
| clospan 和 rowspan        | 合并属性       | 用来合并单元格的                             |

1. 表格提供了HTML 中定义表格式数据的方法。
2. 表格中由行中的单元格组成。
3. 表格中没有列元素，列的个数取决于行的单元格个数。
4. 表格不要纠结于外观，那是CSS 的作用。
5. 表格的学习要求：  能手写表格结构，并且能简单合并单元格。


## 7. 拓展阅读@

### 表格划分结构（了解）

```
对于比较复杂的表格，表格的结构也就相对的复杂了，所以又将表格分割成三个部分：题头、正文和脚注。而这三部分分别用:thead,tbody,tfoot来标注， 这样更好的分清表格结构
```

![thead](https://i.loli.net/2020/12/01/nsR2q5xcAeMjNZF.png)

**注意：**

1. &lt;thead>&lt;/thead>：用于定义表格的头部。用来放标题之类的东西。&lt;thead> 内部必须拥有 &lt;tr> 标签！
2. &lt;tbody>&lt;/tbody>：用于定义表格的主体。放数据本体 。
3. &lt;tfoot>&lt;/tfoot>放表格的脚注之类。
4. 以上标签都是放到table标签中。