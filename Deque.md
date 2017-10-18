# Deque

Deque接口是“double ended queue”的缩写(通常读作“deck”)，即双端队列，支持在队列的两端插入和删除元素，继承Queue接口。大多数的实现对元素的数量没有限制，但这个接口既支持有容量限制的deque，也支持没有固定大小限制的。
Deque接口定义了在两端访问元素的方法，主要包括insert、remove和examine。和Queue定义一样，所有这些方法存在两种形式：一种如果操作失败则抛出异常，另一种则返回一个特殊值(null或false)。后者主要是为有容量限制的队列实现的。
Deque的12种方法总结如下：
Summary of Deque methods
 	             First Element (Head)	            Last Element (Tail)
        Throws exception	Special value	  Throws exception	  Special value
Insert	addFirst(e)	      offerFirst(e)	  addLast(e)	        offerLast(e)
Remove	removeFirst()	    pollFirst()	    removeLast()	      pollLast()
Examine	getFirst()	      peekFirst()	    getLast()	          peekLast()


http://blog.csdn.net/blog_szhao/article/details/23914169
