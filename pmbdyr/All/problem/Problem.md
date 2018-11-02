# **开昕生日愚人**

---

## 以前的版本

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)特别喜欢以前的版本，所以他出了这么一道题来考考你。

### **题目描述**

给你一个数字ID，请你输出这个物品名称。

### **输入格式**

一行一个整数，代表数字ID。

### **输出格式**

一行一个字符串，格式是：9个英文字母+英文半角冒号+物品名称。

### **样例输入**

暂无测试点

### **样例输出**

暂无测试点

### **说明**

数字ID$\leq$50

物品附加参数为0

2018年4月20日就是[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)的生日了。

---

## T2 低级计算器

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)在考试时经常```饭```一些低级的错误，例如他经常把1+1算成1,1$\times$1算成2,2$\times$2算成2，他受不了了，只好请你帮他写一个低级计算器。

### **题目描述**

给你写在```C++```里的一次方程（这样就避免读入"$\times$","$\div$","$\frac{a}{b}$"这种奇奇怪怪的符号），请你解出对应变量的值。

### **输入格式**

第一行有一个整数n和n个字母，分别代表字母及方程个数和变量名。  
接下来n行，每行是一串含变量的一次方程（保证所有字母在等式左边，值在等式右边）。

### **输出格式**

共n行，每行为一个变量（按输入顺序排列）+等号+对应的值。

### **样例输入**

**Input**

> 2 x y
> x+y==6
> x-y==4
> 

### **样例输出**

**OutPut**

> x==5
> y==1
> 

### **说明**

符号只有![+、-](https://cdn.luogu.org/upload/pic/17457.png)和![*、&](https://cdn.luogu.org/upload/pic/17459.png)

保证有解，方便起见n$\leq$5，系数均在-9~9之间。

2018年4月20日就是[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)的生日了。

---

## T3 字符串的值

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)的字符串相关知识不是很好，于是他想看看你的水平怎么样。

### **题目描述**

给你一个字符串，求它的值。

### **输入格式**

一行一个字符串，长度不超过10。

### **输出格式**

一行数，代表它的值。

### **样例输入**

**Input**

> abc
> 

### **样例输出**

**OutPut**

> 294
> 

### **说明**

字符串长度不超过10。

2018年4月20日就是[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)的生日了。

![误差在0.000001内即可通过](https://cdn.luogu.org/upload/pic/17460.png)

---

## T4 二项式展开

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)发现5以内的杨辉三角数可以用$11^n$来计算，当他把这个发现告诉他的数学老师时，他的数学老师Diss了PM。于是PM请你写个程序帮他。

### **题目描述**

请你帮他计算杨辉三角数，并用于输出$(a+b)^n$的展开式。

### **输入格式**

共一行一个整数n。

### **输出格式**

一行一个字符串，为套用帮他计算的杨辉三角数的展开式。（幂数为0时应不输出该项，幂数为1时应省去，系数输出方法同系数）

### **样例输入**

**Input**

> 3
> 

### **样例输出**

**OutPut**

> a^3+3a^2b+3ab^2+b^3
> 

### **说明**

n$\leq$50

2018年4月20日就是[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)的生日了。

---

## T5 三角圆函数

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)喜欢称三角函数为三角圆函数（三角函数又称为圆函数），但他又不会计算，于是他出了此题看看你会不会计算。

### **题目描述**

给你一个三角函数名和```C++```对应配值的类型的数，请你计算出值。

### **输入格式**

一行一个字符串和一个数，分别代表三角函数名和```C++```对应配值的类型的数。

### **输出格式**

一行一个数，代表值。

### **样例输入**

**Input**

> sin 0.785398
> 

### **样例输出**

**OutPut**

> 0.707107
> 

### **说明**

数在小数点后六位以内。

误差在0.000001内即可通过。

2018年4月20日就是[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)的生日了。

---

## T6 无规律数列

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)知道一个数列，他决定将这个毫无规律的数列哪来问你。

### **题目描述**

这个数列的前五个数是$\begin{Bmatrix}0&0&1&1&2& \cdots \end{Bmatrix}$，你需要输出这个数列的第n个数。

### **输入格式**

一行一个整数n。

### **输出格式**

一行一个整数，代表这个数列的第n个数。

### **样例输入**

**Input**

> 6
> 

### **样例输出**

**OutPut**

> 3
> 

### **说明**

由于这个数列太特殊了，于是PM决定让n满足n$\leq$16

2018年4月20日就是[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)的生日了。

