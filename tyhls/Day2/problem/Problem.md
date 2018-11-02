# **退役模拟赛Day2**

---

## T1 谁是最惨的人

**Time:$1000MS$ Memory:$256MB$**

### **题目背景**

[@陈子骏](https://www.luogu.org/space/show?uid=60874)被机惨到爆炸，这一次他的库文件遭殃了，被机房最强机惨王修改了，这下他可就慌了啊，没办法了，只能找你了。

### **题目描述**

机房最强机惨王告诉机房最惨者他隐藏了他的库，由于~~数据太难造~~他们忽略了其他字符，所以他告诉你的内容只有英文。 相比起找回原来的库，他更倾向于手写一个新的。  
现在告诉你一些有关于库$k$的信息。这意味着他记得一串字符$s_i$在库$k$中至少出现了$x_i$次。以及$x_i$个$s_i$在k中出现的位置--$a_{i,1}$，$a_{i,2}$，$a_{i,3}$，$a_{i,4}$，…，$a_{i,x_{i}}$。他记得n个这样的字符串$s_{i}$。  
你要重建出一个符合最强机惨王记得的所有信息的库，如果有多个答案符合要求，取字典序最小的一个。字符串$s_{i}$只包含小写字母。

### **输入格式**

第一行包括一个整数n,代表了最强机惨王所记得的字符串数量。
下面的n行包括有关于这些字符串的信息。第i+1行包括一个非空字符串$s_{i}$，一个正整数$x_{i}$(代表了$s_{i}$在库$k$中出现的次数)，然后是$x_{i}$个正整数$a_{i,1}$，$a_{i,2}$，$a_{i,3}$，$a_{i,4}$，…，$a_{i,x_{i}}$（升序输入），代表了$s_{i}$在库$k$中出现的起始位置。

### **输出格式**

如果可以还原出来，输出满足条件的字典序最小的一行字符串表示库，否则输出机房最惨者的英文首字母缩写大写。

### **样例输入**

**Input 1**

> 14
> include 1 1
> bits 1 8
> std 2 12 31
> ch 1 15
> using 1 17
> namespace 1 22
> int 2 34 41
> main 1 37
> a 3 44 49 55
> b 3 45 50 56
> cin 1 46
> cout 1 51
> endl 1 57
> return 1 61
> 

**Input 2**

> 11
> include 1 1
> bits 1 8
> std 2 12 31
> ch 1 15
> using 1 17
> namespace 1 22
> int 1 34
> main 1 37
> cout 22 41 46 51 56 61 66 71 76 81 86 91 96 101 106 111 116 121 126 131 136 141 146
> n 22 45 50 55 60 65 70 75 80 85 90 95 100 105 110 115 120 125 130 135 140 145 150
> return 1 151
> 

### **样例输出**

**OutPut 1**

> includebitsstdchusingnamespacestdintmainintabcinabcoutabendlreturn
> 

**OutPut 2**

> includebitsstdchusingnamespacestdintmaincoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutncoutnreturn
> 

### **说明**

$1<=n<=10^{5}$，保证字符串$s_{i}$的长度之和不超过$10^{5}$，$1<=a_{i,j}<=10^{5}$，$1<=x_{i}<=10^{5}$，且$x_{i}$的和不超过$10^{5}$。可能存在相同的$s_{i}$。

如果不知道机房最惨者的英文首字母缩写大写，可以查看[博客](https://williampetermatthew.github.io/)的友链。

本题By：[Peter_Matthew](https://www.luogu.org/space/show?uid=59593)

---

## T2 谁是最神的人

**Time:$1000MS$ Memory:$256MB$**

### **题目背景**

由于[@noco](https://www.luogu.org/space/show?uid=60883) rank前3了，NOIp 进队稳了，但他太fake了，以至于每次模拟赛他总是想进一切办法故意不ak。

### **题目描述**

已知他不ak的方法有
1. CE
2. 不打文件输入输出 
3. 故意特判情况输出假答案

每种防ak方法比赛都有一个fake值，他虽然很fake，但希望尽量不被人发现自己的fake，所以希望别人不发现自己fake。

有m场比赛，@sqh 可以将fake 操作分给每场比赛，每场比赛都至少有1次fake操作，至多无上限的fake 操作  
由于方法 1，2太容易被发现fake了，所以定义一个fake常数 fuke，fuke=((每一次1操作的fake值的乘积)加上((每一次2操作的fake值的和)除以2))/1操作次数  
每场比赛的fake值等于该场fake操作值的和减去fuke值的平方  
总比赛fake值为其每场比赛fake值和除以比赛场次  
他当然知道自己每场fake值的和最小等于多少，但他是最神的人，所以他想问问你

### **输入格式**

第一行给出n，m，表示有n次防ak操作，m场比赛  
接下来n行给出两个数 k,i,表示fake方法种类和fake值  

### **输出格式**

一个实数ans（保留两位小数），表示最小总比赛fake值  
如果他太fake了，总fake值（ans）都大于等于19260817.0了，则输出机房最神的人的英文首字母缩写大写  

### **样例输入**

**Input**

> 6 3
> 1 1
> 1 2
> 2 3
> 3 4
> 3 6
> 3 5
> 

### **样例输出**

**OutPut**

> 27.56
> 

### **说明**

fuke = （（1*2）+（3/2））/2

n<=30 , m<=15，i<=10 
保证fuke值在double范围内  

如果不知道机房最神的人的英文首字母缩写大写，可以查看[博客](https://williampetermatthew.github.io/)的友链。

本题By：[Shirai_Kuroko](https://www.luogu.org/space/show?uid=75939)

---

## T3 谁是退役的人

**Time:$1000MS$ Memory:$256MB$**

### **题目背景**

颓废是退役的根源！！！

### **题目描述**

[@Shirai_Kuroko](https://www.luogu.org/space/show?uid=75939)、[@树下](https://www.luogu.org/space/show?uid=60871)、[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)是机房最颓的三个人。在平时他们会颓废，当然也会学一些知识。当他们太颓废的时候就会退役。  
众所周知，[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)喜欢Splay树，所以他构建了一棵树来模拟三人的退役过程。  
[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)是这样进行模拟的：首先为三个人每人建一棵二叉树来模拟他们的心理，然后在其中一些叶结点上分别放上学习和颓废两种选择之一，其中，学习记为1，颓废记为负整数，不同的负整数表示不同的颓废种类。  
三个人各自有一个计划列表，在计划列表上，每天，[@Shirai_Kuroko](https://www.luogu.org/space/show?uid=75939)、[@树下](https://www.luogu.org/space/show?uid=60871)和[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)各自会选择一个节点。每天每个人选择的节点所在的被染色的子树的最顶端的节点会执行一次rotate操作，然后它到达的新节点为根的子树会被全部染成这种颜色。有时被选择的节点没有被染色，这时这个人会很不高兴而什么都不做。  
当一个人颓废过度之后，他就会直接退役。一个人颓废过度有如下两种情况：1.所有颓废子树的根的深度都浅于学习子树的根。2.学习操作所在的子树沦陷。当满足以上两种条件的至少一个时，这个人就会退役。当有人退役的时候，其他人就不敢继续颓废也就不会再有人退役。  
现在[@Shirai_Kuroko](https://www.luogu.org/space/show?uid=75939)和[@树下](https://www.luogu.org/space/show?uid=60871)列好了他们的计划表交给了[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)，而且[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)构建好了他们原本的二叉树形态。但是[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)太蒟蒻了不会进行这么复杂的模拟，于是他把这些数据交给了你，而你的任务就是找到谁是退役的人。  

### **输入格式**

第一行给出三个正整数a,b,c，分别表示三个人的二叉树的节点数。  
接下来的a-1行，每行有两个整数x,y，表示[@Shirai_Kuroko](https://www.luogu.org/space/show?uid=75939)的二叉树上存在的父子关系，x是y的儿子，节点标号从1开始。你可以认为第一个被确立为某点的儿子的点是其左儿子，因为[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)就是这么认为的。  
接下来的b-1行及再接下来的c-1行同理，表示[@树下](https://www.luogu.org/space/show?uid=60871)和[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)的二叉树上存在的父子关系。  
接下来的一行给出三个正整数A,B,C，分别表示三个人初始染色节点的个数  
接下来的A行、B行、C行每行两个正整数p、t，分别给出[@Shirai_Kuroko](https://www.luogu.org/space/show?uid=75939)、[@树下](https://www.luogu.org/space/show?uid=60871)和[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)的初始染色节点的信息，表示p节点被染为t色。  
接下来的一行给出一个整数m，表示三人还有m天的时间可以安排。  
接下来的m行，每行三个整数wa，wb，wc，分别表示三人当天要操作的节点。

### **输出格式**

若有人退役，则在第一行输出他/他们退役的时间，接下来至多三行，表示退役的人。若[@Shirai_Kuroko](https://www.luogu.org/space/show?uid=75939)退役，则输出SK，若[@树下](https://www.luogu.org/space/show?uid=60871)退役，则输出TCK，若[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)退役，则输出PPT。若多个人同一天退役，则按照题目中三人的顺序输出三个人对应的答案。  
若直到最后也没有人退役，请在第一行输出世界最强OI教练的英文首字母缩写大写，在接下来的三行中按照题目中三人的顺序输出他们的树上被染成学习节点的节点数。

### **样例输入**

**Input**

> 5 5 5
> 1 2
> 3 2
> 4 1
> 5 1
> 1 2
> 3 2
> 4 1
> 5 1
> 1 2
> 3 2
> 4 1
> 5 1
> 2 2 2
> 4 1
> 5 -1
> 4 1
> 5 -1
> 4 1
> 5 -1
> 3
> 4 4 5 
> 5 5 4
> 5 5 4
> 

### **样例输出**

**OutPut**

> 1
> PPT
> 

**样例解析**

> [@Shirai_Kuroko](https://www.luogu.org/space/show?uid=75939)、[@树下](https://www.luogu.org/space/show?uid=60871)准备先学习再颓废，而[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)准备先颓废再学习，不过由于第一天的时候[@asdfghjkl123](https://www.luogu.org/space/show?uid=61819)的所有颓废子树的根的深度都浅于学习子树的根，而且学习的子树已经沦陷，所以他直接退役了，之后也没人敢再颓废了。

### **说明**

对于100%的数据，保证:  
3<=a,b,c<=1000;  
x,y<=树的大小;  
1<=A,B,C<=叶子结点个数;  
0<|t|<=min(30,树的大小)，且保证对于每个人，他自己的所有t值不重复（包括1）。  
保证p为叶子结点且至多只会被一次染色。  
1<=m<=1000;  
1<=wa,wb,wc<=a,b,c。

如果不知道世界最强OI教练的英文首字母缩写大写，可以查看[博客](https://williampetermatthew.github.io/)的友链。

本题By：[asdfghjkl123](https://www.luogu.org/space/show?uid=61819)
