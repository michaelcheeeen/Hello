## 静态代理、动态代理


### 基本概念
静态代理通常只代理一个类，动态代理是代理一个接口下的多个实现类

###  区别
静态代理事先要知道代理的是什么 ，而动态代理不知道要代理什么东西，只有在运行时才知道。  
动态代理是实现JDK里面的InvocationHandler接口里面的invoke方法，但注意的是代理的是接口，也就是说你的业务类必须要实现接口，通过Proxy里的newProxyInstance得到代理对象。

### 举例
AOP编程就是基于动态代理实现的，比如著名的Spring框架、Hibernate框架等等都是动态代理的使用例子

### 补充
还有一种动态代理CGLIB，代理的是类，不需要业务继承接口，通过派生的子类来实现代理。通过在运行时，动态修改字节码达到修改类的目的。  




