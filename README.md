## 2018/3/25  ChangeLogs
1. 初始化仓库，其实这份源码之前有阅读过一点,有一些注释现在正是开始同步写博客分析 Java8 源码
2. 博客地址:[博客园](http://www.cnblogs.com/lwen/)
           [个人博客](https://lwenxu.coding.me)
           [简书](https://www.jianshu.com/u/78464cccc621)
           [CSDN](https://blog.csdn.net/Greek_xpf)
### ArrayList
1. ctor-3
2. get
3. set
4. add-2
5. remove-2
6. clear 
7. addAll
8. write/readObject
9. fast-fail
10. subList
11. iterator
12. forEach
13. sort
14. removeIf

### Vector
different with ArrayList


## 2018/3/26  ChangeLogs

### LinkedList
1. ctor-2
2. addFirst
3. addLast
4. addAll
5. add
6. indexOf
7. lastIndexOf
8. peek 获取第一个元素，是 null 就返回 null
9. peekFirst/Last  获取第一个最后一个元素
10. poll 删除第一个元素并返回 没有返回 null
11. pollFirst/Last 
12. offer 调用了 add
13. offerFirst/Last
14. push
15. pop
16. set
17. remove(noArgs) == removeFirst  继承自 deque
18. remove(E e) 查找删除
19. read/writeObject  还是手动的序列化，原因一样，直接序列化元素而没有 pre/next

### HashMap
1. ctor-4
2. put/putVal
4. resize
5. putAll/putMapEntries
6. get/getNode/containsKey 
7. remove/removeNode/clear
8. containsValue
9. read/writeObject

### LinkedHashMap
1. ctor-5  最重要的能实现 LRU 的是设置 accessOrder 的那个
2. afterNodeRemoval
3. afterNodeInsertion
4. afterNodeAccess
5. containsValue
6. get
7. removeEldestEntry

## 2018/3/27  ChangeLogs

### HashSet
1. ctor-5
2. add
3. remove
4. read/writeObject

### LinkedHashSet
1. ctor-3

### ConcurrentHashMap
1. ctor-4 延时加载

1. size
2. sumCount
3. get
4. containsKey/Value（Traverser对象）
5. put/putVal/initTable
6. tableAt/casTableAt/setTableAt
7. tryPresize
8. helpTransfer
9.  transfer
10. treeifyBin
11. remove/replaceNode
12. clear
13. read/writeObject

## 2018/3/29  ChangeLogs

Synchronized keyword   javap -c/v 

## 2018/3/30  ChangeLogs
### Lock interface
1. ctor-2
2. lock
3. lockInterruptibly
4. tryLock
5. tryLock(time)
6. unlock
7. newCondition

### Condition/Node inner class in AQS
1. await
2. notify
3. notifyAll

### AQS
1. get/setState
2. release/tryRelease/unparkSuccessor/fullyRelease
3. acquire/tryAcquire/addWaiter/tryQueued
4. acquireShared
5. releaseShared

## 2018/4/1  ChangeLogs
### Semaphore
1. ctor-2
2. require
3. release

## 2018/4/3  ChangeLogs
1. ctor-1
2. await/tryAcquire
3. countDown/tryRelease