## List -- 实现List接口的集合类，特点是有序可重复: 添加的顺序和遍历的顺序一致

Leetcode: 2, 55, 57

http://www.cnblogs.com/fingerboy/p/5478073.html

____________________________________________

**ArrayList - 顺序存储结构的表**

http://www.cnblogs.com/bayes/p/5474728.html

- 该类的内部维护了一个集合数组，因此查询速度快，但是增删速度较慢，因此用于查询较多写入删掉少的场景中

- Array和ArrayList的区别:

  http://blog.qianlicao.cn/translate/2016/03/09/array-vs-arraylist/
  
  Array是静态的，Array被初始化之后，数组长度就不能再改变了。ArrayList是可以动态改变大小的。那么，什么时候使用Array，什么时候使用ArrayList?答案是：当我们不知道到底有多少个数据元素的时候，就可使用ArrayList；如果知道数据集合有多少个元素，就用Array。但Array和ArrayList的查找时间复杂度都是O(1).
  
  Array.length(); ArrayList.size();

- 注意：ArrayList类只支持对象类型，不支持 基础数据类型。就是说ArrayList对象只能存放对象，不能存放基础数据类型的数据。

- 获取链表中指定位置处的元素 E.get(int index)



____________________________________________

**LinkedList - 链式存储结构的表**

http://www.cnblogs.com/skywang12345/p/3308807.html

LinkedList.peek() - 此方法返回此列表的头元素，或null，如果此列表为空 （但不移除）
LinkedList.remove() - 此方法返回并移除此deque队列表示的队列的头部
