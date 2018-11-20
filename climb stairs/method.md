**问题**
假设你现在正在爬楼梯，楼梯有n级。每次你只能爬1级或者2级，那么你有多少种方法爬到楼梯的顶部？

**思路**

根据题意，定义两个长整型p和q,如果为1则返回1，否则返回2；然后用for循环将第一个值p赋给tmp，其次将第二个值q赋给p,以后每一次赋值都将得到的最新的F(n)赋给p,从后面语句可以看出,q储存的为最新的F(n)，从3开始的值第一层数据 tmp是1，2，3，4，5，……第二层 p是2，3，5，7，12，……  第三层q是3，5，7，12，21，……；最后取地址输出该整数。 


