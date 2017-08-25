**int 范围： (Integer.MAX_VALUE) 2^31 - 1 ~ -2^31 (Integer.MIN_VALUE)**

**long 范围：2^63 - 1 ~ -2^63**

_________________________________

**return a? b:c means 
if(a) b;
else c;**

_________________________________

http://www.runoob.com/java/java-operators.html

**java中有三种移位运算符**

"<<"  左移运算符，num << 1,相当于num乘以2

">>" 右移运算符，num >> 1,相当于num除以2

">>>"  无符号右移，忽略符号位，空位都以0补齐

"<< =" 左移位赋值运算符	C << = 2等价于C = C << 2

">> ="	右移位赋值运算符	C >> = 2等价于C = C >> 2

_________________________________

http://www.cnblogs.com/Hugooscar/p/6043713.html

length:用于获取数组长度。

length():用于获取字符串长度。

size():用于获取泛型集合有多少个元素。

eg:
```java
Collection<String> col = new ArrayList<String>();
col.add("Hello");
col.add("World");
col.add("Java");
int sizeCol = col.size();//此处sizeCol=3
System.out.println("Col size:"+sizeCol);
```
