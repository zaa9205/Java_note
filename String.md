# String

Leetcode: 006.ZigZag Conversion; 043.Multiply String; 067.Add Binary; 214.Shortest Palindrome
_______________________________
String: http://www.cnblogs.com/YSO1983/archive/2009/12/07/1618564.html

StringBuffer, StringBuilder: 

http://blog.csdn.net/u010575093/article/details/50728538

http://www.cnblogs.com/Qian123/p/5193076.html

对于StringBuffer同样适用：
StringBuilder.append(); - 在String的后面直接增加

StringBuilder.toString(); -转为string

StringBuilder.reverse(); -倒序一遍

1. String、StringBuffer、StringBuilder区别 
答：Java平台提供了两种类型的字符串：String和StringBuffer/StringBuilder，它们可以储存和操作字符串。 
而StringBuffer/StringBuilder类表示的字符串对象可以直接进行修改。 
StringBuilder是Java 5中引入的，它和StringBuffer的方法完全相同，区别在于它是在单线程环境下使用的，因为它的所有方面都没有被synchronized修饰，因此它的效率也比StringBuffer要高。

2. 面试题 - 什么情况下用+运算符进行字符串连接比调用StringBuffer/StringBuilder对象的append方法连接字符串性能更好？ 
答：如果使用少量的字符串操作，使用 (+运算符)连接字符串； 
如果频繁的对大量字符串进行操作，则使用 
1：全局变量或者需要多线程支持则使用StringBuffer； 
2：局部变量或者单线程不涉及线程安全则使有StringBuilder。
 
那为什么我们很少见到StringBuilder呢？原因很简单，因为我们有时候很难确定我们创建的系统会不会是多线程的，如果考虑到以后扩展的可能性，则更难确定，所以我们更愿意使用StringBuffer，因为它是线程安全的，不用担心以后扩展。

_______________________________
## String int 互相转换
## int -> String

int i=12345;

String s="";

第一种方法：s=i+""; 

第二种方法：s=String.valueOf(i);

这两种方法有什么区别呢？作用是不是一样的呢？是不是在任何下都能互换呢？

## String -> int

s="12345";

int i;

第一种方法：i=Integer.parseInt(s);

第二种方法：i=Integer.valueOf(s).intValue();

这两种方法有什么区别呢？作用是不是一样的呢？是不是在任何下都能互换呢？

以下是答案：

第一种方法：s=i+"";  //会产生两个String对象

第二种方法：s=String.valueOf(i); //直接使用String类的静态方法，只产生一个对象

第一种方法：i=Integer.parseInt(s);//直接使用静态方法，不会产生多余的对象，但会抛出异常
第二种方法：i=Integer.valueOf(s).intValue();//Integer.valueOf(s) 相当于 new Integer(Integer.parseInt(s))，也会抛异常，但会多产生一个对象
