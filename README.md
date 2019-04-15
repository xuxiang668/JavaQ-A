# JavaQ-A
Java面试问题大全

Java SE部分
一、Java基础
1. 为什么重写equals还要重写hashCode方法?
答：重写equals是为了判断两个自定义对象是否相等，然而如果我们用自定义的对象充当HashMap的key时，会出现一种情况：我们认为的同一对象，因为哈希值不同导致用这个对象取不到HashMap中的值，或者会导致在HashMap中存了两个key。所以才需要进行hashCode方法的覆盖。
