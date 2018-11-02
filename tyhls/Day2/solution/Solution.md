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

### **简要题解**

[LuoguT53816](https://www.luogu.org/problemnew/show/T53816):

按思路模拟即可。

要点：
1. 注意'\0'会影响字符串输出
2. 后输入的字符串应覆盖前面输入的字符串


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

### **简要题解**

可以观察到，数据范围贼小，所以首先，有耐性和心态好的人可以通过极其优秀的暴力过掉，然后呢，最强的那个人还考虑了状压DP的做法~~但我不会~~但数据小还能想到的办法当然是随机算法——模拟退火！但由于数据忒小了，其实写个真随机性算法每次随机数据排列分组贪心然后取最优即可


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

### **简要题解**

Splay？Rotate？不不不！这些都是蒟蒻出题人吓唬做题人的道具而已。

实际上 rotate 操作在这里起到的作用等价于将节点的父节点染为相同颜色。原因就是在rotate(x)之后，x 的原父节点 y 的另一个儿子变成了 x 的后代，而 y 变成了 x 的后代。然后它们都被重新染色。而且这种染色对于其他的子树没有任何影响。

学习子树被覆盖只需判断其祖先们有一个被覆盖。当然，由于数据范围过小，所以也可以遍历子树进行赋值。而对于另一种情况，可以打标记啊什么的，但是我不会写……而且数据太小，所以每次就暴力染色即可。

首先要维护好一棵树的基本信息，比如深度和子树大小什么的。

直接写三个人三棵树可能会比较难受，所以可以先写一个人一棵树，然后把数组加一维得到三个人三棵树的写法。


如果不知道世界最强OI教练的英文首字母缩写大写，可以查看[博客](https://williampetermatthew.github.io/)的友链。

本题By：[asdfghjkl123](https://www.luogu.org/space/show?uid=61819)
