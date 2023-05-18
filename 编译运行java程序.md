## java程序编译运行流程
以hello.java为例：  
java源文件（hello.java）->javac.exe hello.java(java编译器)->java字节码文件(hello.class)  
->java.exe hello(java虚拟机(jvm)装载java字节码文件执行java程序)  
注意执行java字节码文件时不带后缀，若带上后缀如hello.class，  
jvm会去寻找名为hello.class的类，但我们只有名为hello的类，程序报错

## java源文件注意事项
1. java程序的执行入口为main()函数
2. 一个java源文件最多有一个public类，非public类个数不限
3. 若java源文件包含一个public类，则文件名必须以该类名命名 hello.java中的public类的类型应是hello
4. main函数可以在public类中，也可以在非public类中，假设hello.java中有三个类，  
hello、dog和cat，hello是public类，三个类中均有main函数，在编译hello.java时会产生三个java字节码文件 hello.class、dog.class和cat.class，  
三个文件分别对应三个类，当用jvm执行相应的java字节码文件时  
程序便执行相应的类中的main函数，如java dog便会执行dog类中的main函数
