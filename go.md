# GO Interview Question

### 1、两个groutine交替打印字母和数字

### 2、Go中的空结构体有什么用处

- type set map[string]struct{} 用来实现集合

- 不发送数据的channel
- 只包含方法的结构体

### 3、interface类型能否比较

interface类型中包含动态类型和动态值，只有当动态类型和动态值均相等时才是相等

### 4、defer执行顺序

后进先出 

 顺带提了go defer在命名与匿名返回值函数中的差异，如果return x，x并没有在函数声明中定义，那么在return时会创建一个临时变量tmp = x来返回，所以defer中对x的操作不会在return中生效，如果是命名返回值函数就不会存在这一个问题，因为不需要去创建临时变量。

### 5、无缓冲channel和有缓冲channel区别

### 6、谈谈对Go协程的理解

### 7、Go中如何面向对象？

继承——组合，多态——interface duck模型，封装——首字母大小写