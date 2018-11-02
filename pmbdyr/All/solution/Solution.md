# **开昕生日愚人**

---

## 以前的版本

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)特别喜欢以前的版本，所以他出了这么一道题来考考你。

### **题目描述**

给你一个数字ID，请你输出这个物品名称。

### **简要题解**

[LuoguT27508](https://www.luogu.org/problemnew/show/T27508):

本题所指的以前的版本是指Minecraft的以前的版本。数字ID指的是1.7及之前的版本，当时使用数字ID，之后的版本则使用“minecraft:xxx”的方式表示物品ID，其实物品附加参数不为0的物品ID是一样的，所以说明里的那句是为了提示而写的。

0pts：打表使用“Minecraft”或“：”输出

98pts：没有打ID为0时的表。

100pts：避开上述错误打50以内的表即可。

---

## T2 低级计算器

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)在考试时经常```饭```一些低级的错误，例如他经常把1+1算成1,1$\times$1算成2,2$\times$2算成2，他受不了了，只好请你帮他写一个低级计算器。

### **题目描述**

给你写在```C++```里的一次方程（这样就避免读入"$\times$","$\div$","$\frac{a}{b}$"这种奇奇怪怪的符号），请你解出对应变量的值。

### **简要题解**

[LuoguT27516](https://www.luogu.org/problemnew/show/T27516):

本道题是所有这6题中最难的一道，因为为了愚人，让人觉得简单而放到了第二题的位置。

60pts：写出多元一次方程组求解代码。

100pts：注意在题目的说明里有两张图片![+、-](https://cdn.luogu.org/upload/pic/17457.png)和![*、&](https://cdn.luogu.org/upload/pic/17459.png)，这里的两张图片用审查元素可以看到说明分别是“```+、-```”和“```*、&```”，而用到```*```和```&```的只有```C++```中的指针，所以在60pts的代码基础上加上指针的判断即可AC。

---

## T3 字符串的值

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)的字符串相关知识不是很好，于是他想看看你的水平怎么样。

### **题目描述**

给你一个字符串，求它的值。

### **简要题解**

[LuoguT27521](https://www.luogu.org/problemnew/show/T27521):

简单的题？非也非也。

6pts：按正常题意输出几个字符之和。

74pts：字符中有几个例如'NUL'、'TAB'、'EOF'之类神奇的单字符，读到这些要输出对应的值，例如'NUL'是0，则读到"NUL"时应输出0。加上6pts的判断，即可得到84pts。

100pts：看说明下面好像白的地方比较多，用审查元素可以看到这张图片![误差在0.000001内即可通过](https://cdn.luogu.org/upload/pic/17460.png)，它附有一段说明：“误差在0.000001内即可通过”，这是怎么回事呢？在math.h库中，存在13个已定义的常数，例如M_E，M_PI，M_PI_2之类的常数，所以在读到时要输出值"M_E"，要输出小数点后6位以内对应的值2.718282。再加上84pts的程序，就可以得到100pts。

---

## T4 二项式展开

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)发现5以内的杨辉三角数可以用$11^n$来计算，当他把这个发现告诉他的数学老师时，他的数学老师Diss了PM。于是PM请你写个程序帮他。

### **题目描述**

请你帮他计算杨辉三角数，并用于输出$(a+b)^n$的展开式。

### **简要题解**

[LuoguT27522](https://www.luogu.org/problemnew/show/T27522):

此题用了二项式定理，不知道可自行百度。

20pts：就是表面上看的输出展开的字符。

100pts：5以内杨辉三角数可以按$11^n$计算？$n\leq4$是没错，但是n==5时为161051，显然不是，那是不是我写错了呢？当然不是。所以你需要做的是按照这个规律输出。当然显然是没法按照$11^n$乘算的，所以我们只需要先算出杨辉三角数，然后再从后往前传大于10的数即可，多于总数时要多输出一个常数。

---

## T5 三角圆函数

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)喜欢称三角函数为三角圆函数（三角函数又称为圆函数），但他又不会计算，于是他出了此题看看你会不会计算。

### **题目描述**

给你一个三角函数名和```C++```对应配值的类型的数，请你计算出值。

### **简要题解**

[LuoguT27523](https://www.luogu.org/problemnew/show/T27523):

由于本题比较复杂，不再详细多少分对应什么问题或算法了，因为会出的错误千奇百怪，这其实是由于对“三角函数”的概念不是非常具体，我在题目中也说了，“三角函数”又叫“圆函数”。  
这里要科普下：三角函数可不止包括sin、cos和tan，还不止包括cot、sec和csc，更不止包括asin、acos、atan、acot、asec和acsc。  
有人会问了，那还有什么，其实还有很多，这题里面还有双曲三角函数sinh、cosh...及其反函数asinh、acosh...当然这题我皮了一下，还写了他们的全称，sine、tangent、secant、arc（例如arcsine）、hyperbolic（例如hyperbolicsine）。所以打字符表，写函数即可AC。  
因为正矢（versin、vercosin）、余矢（coversin、covercosin）、半正矢（haversin、havercosin）、半余矢（hacoversin、hacovercosin）、外正割（exsec）和外余割（excsc）看完百科后太好推了，所以我就没有出这组数据。  
最后附赠一段本题出题的参考链接：  
[三角函数](https://baike.baidu.com/item/%E4%B8%89%E8%A7%92%E5%87%BD%E6%95%B0/1652457)| [反三角函数](https://baike.baidu.com/item/%E5%8F%8D%E4%B8%89%E8%A7%92%E5%87%BD%E6%95%B0)  
[双曲三角函数](https://baike.baidu.com/item/%E5%8F%8C%E6%9B%B2%E5%87%BD%E6%95%B0)|[反双曲三角函数](https://baike.baidu.com/item/%E5%8F%8D%E5%8F%8C%E6%9B%B2%E5%87%BD%E6%95%B0)

---

## T6 无规律数列

**Time:$1000MS$ Memory:$256MB$ SpecialJudge**

### **题目背景**

[@Peter_Matthew](https://www.luogu.org/space/show?uid=59593)知道一个数列，他决定将这个毫无规律的数列哪来问你。

### **题目描述**

这个数列的前五个数是$\begin{Bmatrix}0&0&1&1&2& \cdots \end{Bmatrix}$，你需要输出这个数列的第n个数。

### **简要题解**

[LuoguT27533](https://www.luogu.org/problemnew/show/T27533):

拿到这组数蒙了？为了方便大家找规律，我在出样例时特意给大家又多往后延伸了一位n==6时的样例。

0pts：知道我的题【U22412 [PP游戏#5 种树游戏（Tree Game）](https://www.luogu.org/problemnew/show/U22412)】的朋友可能会根据$3\leq n \leq 6$时的数列$\begin{Bmatrix}1&1&2&3& \cdots \end{Bmatrix}$以为是我PP游戏#5中n==2时的斐波那契数列然后一看$n\leq16$就打表输出，结果就全WA了。

40pts：在这里科普的是，这个数列真的是个毫无规律的数列，但也并不是完全没有，真正的做法是百度一下这个数列，然后就出来了一个[视频链接](http://v.youku.com/v_show/id_XMTMxNzQ1Nzg2OA==.html)，在这个视频中，国外YouTube的numberphile数学家讲解了这个数列是素纽结的结数序列，并把这个数列给到了$n\leq10$时的值，打表提交即可得到40pts。

70pts：显然这题数据点是$7\leq n\leq16$，所以发动广大网友的力量，我们成功的在某贴吧中找到了$n\leq13$时的值，打表提交即可得到70pts。

100pts：题解到这里，不仅会有人会问，都已经翻遍网络了，还没有AC，PM你的后3个点是不是故意不让人过的所以乱造的数据啊？这里我要回复：不，那是因为你没有访问维基百科找[Prime_knot素纽结](https://en.wikipedia.org/wiki/Prime_knot)，这才是真正的答案来源，可以看到连维基百科都只把数列给到$n\leq16$，说明这是多么的无规律，所以~~毒瘤的~~我当然不会放过了，最后打表提交即可AC。
