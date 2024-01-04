# java对象


## 什么是Object？
是超级类。所有的类都直接或间接的继承Object类，一个类不继承其他类，将默认继承Object类

## Object的toString方法
我们通常重写这个方法,来实现返回对象的所有属性的具体信息

## Object的equals方法
1. 对象用==比较的是内存地址。如果要比较对象中所有属性是否相等，需要重写此方法
2. 一般在重写equals方法时会同时重写hashCode方法

## 如何创建对象
创建对象也叫实例化对象
```Java
类名 对象名 = new 类名();
```

## 什么是实例化对象？

1. 实例化对象是指通过类来创建具体的对象实例。在面向对象编程中，类是对象的抽象描述，而对象是类的具体实例。实例化对象的过程包括使用构造方法为对象的各个实例变量分配内存并赋初始值，然后返回一个引用声明的对象变量。这个对象变量保存在栈内存中，而对象的实体（即数据成员）保存在堆内存中。
2. 通过实例化对象，我们可以使用类的功能，并且可以访问对象的成员函数和普通函数。实例化对象是面向对象编程中的重要概念之一，它使得我们可以创建出更加灵活、可重用和可维护的软件系统。
3. 子类实例化会先初始化父类，父类初始化并不是又创建一个父类对象，而是把父类中定义的相关属性都初始化，因为这些属性子类对象也是拥有的。所以，为了保证子类对象的完整性，要从最底层的父类开始，逐级初始化，所有初始化都完成后才会生成一个完整的子类对象。（也就是要区分开实例化和初始化）

## 抽象类能实例化对象吗？

抽象类不能被实例化。因为抽象类中可能包含抽象方法，这些方法没有具体的实现，所以不能直接创建抽象类的实例。但可以通过继承和实现抽象类中的抽象方法来创建具体类的实例。

## 对象的序列化和反序列化

对象的序列化和反序列化是两个过程，可以将对象的状态信息转换为字节流，反之亦然。

1. 序列化是将对象的状态表示为字节序列的过程，可以通过网络传送、存储到文件中或者使用其他的持久化技术，如数据库等。序列化后的字节流可以被传输给远程系统，并在那里重新构造成原始对象。
2. 反序列化是将字节流转化为对象的过程，是对象序列化的逆过程。通过反序列化操作能够在接收端恢复出与发送端相同的对象。