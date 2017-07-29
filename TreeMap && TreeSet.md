# TreeMap

http://wiki.jikexueyuan.com/project/java-enhancement/java-twentyseven.html

TreeMap 基于二叉树，可以保持Key的大小顺序，搜索的时间复杂度为O(lgn)

_____________________________________________________________

# TreeSet

TreeSet <Integer/Long> set = new TreeSet<>();

Integer --> int;

Long --> long;

**Leetcode: 220**

http://wiki.jikexueyuan.com/project/java-enhancement/java-twentyeight.html

我们知道 TreeMap 是一个有序的二叉树，那么同理 TreeSet 同样也是一个有序的，它的作用是提供有序的 Set 集合。


API：

ceiling：返回此 set 中大于等于给定元素的最小元素；如果不存在这样的元素，则返回 null。

floor：返回此 set 中小于等于给定元素的最大元素；如果不存在这样的元素，则返回 null。
