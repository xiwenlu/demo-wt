# jdk新特性

## jdk1.7新特性
1. switch 中可以使用字符串。
2. 即泛型实例化类型自动推断。(`<>`这个玩意儿的运用`List<String> tempList = new ArrayList<>();` )
3. 新增一些取环境信息的工具方法 . (比如 获取jre  目录的方法)
4. 新list 初始化数据的方式。（ `final List<Integer> piDigits = [ 1,2,3,4,5,8 ]; `）

## jdk1.8新特性
1. 接口里面的方式可以用 default 方法而且该方法,可以在接口定义方法体。
2. Lambda 表达式让字符串排序更简单。 b.compareTo(a));
3. 采用双：：来调用静态变量，和构造函数。
4. 提供了多个函数接口。
5. 提供了多个注解。

## jdk1.9新特性
1. 轻量级 JSON API。（对json的操作更简单了）
2. 钱和货币的API （java  jdk1.9 提供了一些操作 钱 的方法）
3. 改善锁争用机制（增加了 单个进程所能操作的线程数  JVM的极限吞吐量显著提升 ）
4. 代码分段缓存（jvm虚拟机能缓存了）       
   （当某段代码被大量重复执行的时候, 虚拟机会把这段代码编译成机器码(native code)并储存在代码缓存里面, 进而通过访问缓存中不同分段的代码来提升编译器的效率.）
5. 智能Java编译, 第二阶段。提升了目前jdk工具的编译性能。
   （改进javac并让其成为取代目前JDK编译工具javac的Java默认的通用编译工具.）