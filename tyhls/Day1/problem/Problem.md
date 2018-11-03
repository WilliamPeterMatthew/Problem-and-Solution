# **退役模拟赛Day1**

---

## T1 高一机惨着你

**Time:$1000MS$ Memory:$256MB$**

### **题目背景**

[@_WA自动机](https://www.luogu.org/space/show?uid=48711)是一位高一神犇，他最喜欢机惨别人。某一天，他觉得机惨别人AK IOI十分没有意思，于是他决定机惨别人一些奇妙的东西。

### **题目描述**

他会机惨不确定个数次别人，每次机惨两个人，每个人他会机惨一行奇妙的东西，你需要回答他被机惨两人的结果。

### **输入格式**

每组数据三行，以次数的序数词起头一行，以"inf"时结束，接下来两行为他机惨的奇妙的东西。

### **输出格式**

每组数据输出一行，如果两人结果不一致，输出机惨结果比较，否则输出机房最强机惨王的英文首字母缩写大写。

### **样例输入**

**Input 1**

> first
> sqhaklenoiphaoinoiioiacmdengdeng
> lmdcaishizuiqiangwangzhe
> second
> woshilouxiadebaba
> woshiloushangdeerzi
> inf
> 

**Input 2**

> first
> wotaiqiangle2333
> woakleioihahahaha
> second
> helaoshitebiedeshuaile
> golaoshiyehenshuai
> inf
> 

### **样例输出**

**OutPut 1**

> bigger
> less
> 

**OutPut 2**

> less
> bigger
> 

### **说明**

数据最多不超过100组，由于他可能随时被抓，所以他不会发送超过1000长度的奇妙的东西。

如果不知道机房最强机惨王的英文首字母缩写大写，可以查看[博客](https://williampetermatthew.github.io/)的友链。

本题By：[Peter_Matthew](https://www.luogu.org/space/show?uid=59593)

---

## T2 高三吊打着你

**Time:$1000MS$ Memory:$256MB$**

### **题目背景**

众所周知，[@Kirin](https://www.luogu.org/space/show?uid=34849)是一位大神犇，在2018.10.26的比赛中又AK虐场了，终于引来了众怒。你和机房的其他人决定一起打他，然而机智的大佬早已躲入了一个神奇的迷宫中，为了追捕（并打他），你也进入到了迷宫中。

### **题目描述**

你现在在（x，y）位置，大佬躲在（1,1）的位置,在这个奇怪的迷宫中，你只能以“日”字或者“田”字走，现在你想知道，你追到大佬的最小步数，若不能请输出机房清华爷的英文首字母缩写大写。（由于大佬太懒了，所以他不会动）

### **输入格式**

两个整数，x，y

### **输出格式**

追到大佬的最小步数，若不能请输出机房清华爷的英文首字母缩写大写。

### **样例输入**

**Input 1**

> 12 16
> 

**Input 2**

> 18 10
> 

### **样例输出**

**OutPut 1**

> 8
> 

**OutPut 2**

> 9
> 

### **说明**

x，y小于20

如果不知道机房清华爷的英文首字母缩写大写，可以查看[博客](https://williampetermatthew.github.io/)的友链。

本题By：[陈子骏](https://www.luogu.org/space/show?uid=60874)

---

## T3 高二退役的你

**Time:$1000MS$ Memory:$256MB$**

### **题目背景**

C蒟蒻在高一的时候掉入了OI这个无底坑中，在gay机房中安静的搞切题。终于在高二的时候迎来了转机的机会。

### **题目描述**

S神[@noco](https://www.luogu.org/space/show?uid=60883)有两套题，a和b，每套题均有n道，每一道题有一个固定的难度。S神要求C蒟蒻[@cs18](https://www.luogu.org/space/show?uid=59934)在两套题中共AC p道即可。

可就在这时却迎来了X神[@_WA自动机](https://www.luogu.org/space/show?uid=48711)的阻挠，X神通过这两套题构造了一套新题c，使得难度cij=ai * bj（你MD一下吧）。X神要求C蒟蒻AK新题，但由于C蒟蒻实在太蒟了，只能在新题中使用S神的神器划分出一个尽可能大的矩形，使得该划分出的区间中题的总难度不大于C蒟蒻的能力上限max，问C蒟蒻是否能AC p道题

### **输入格式**

第一行为三个整数n，p，max，

n表示最初始S神两套题各自的长度；

p表示S神对C蒟蒻的要求；

max表示C蒟蒻的能力上限。

第二行和第三行各有n个数，为最初始S神两套题各自的难度。

### **输出格式**

如果C蒟蒻能够达到S神的要求，输出C蒟蒻共能AC的最多题数；

否则输出~~gay~~机房中最蒟蒻的人的英文首字母缩写大写

### **样例输入**

**Input 1**

> 3 3
> 1 2 3
> 1 2 3
> 9
> 

**Input 2**

> 5 1
> 5 4 2 4 5
> 2
> 5
> 

### **样例输出**

**OutPut 1**

> 4
> 

**OutPut 2**

> 1
> 

### **说明**

n$\leq$50，其余数据均在$10^5$的范围内。

如果不知道~~gay~~机房中最蒟蒻的人的英文首字母缩写大写，可以查看[博客](https://williampetermatthew.github.io/)的友链。

本题By：[cs18](https://www.luogu.org/space/show?uid=59934)