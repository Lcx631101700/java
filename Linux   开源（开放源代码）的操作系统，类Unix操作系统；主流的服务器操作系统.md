Linux   开源（开放源代码）的操作系统，类Unix操作系统；主流的服务器操作系统
计算机的分类：
       1.PC机：个人电脑
       2.服务器：处理大数据请求的高性能的计算机
       3.智能终端：手机、IPAD、掌上电脑、可视电话....
       4.嵌入式设备：除了上面3种意外带CPU的
Windows：PC机
Linux：服务器、智能终端、嵌入式设备
Java主要是用于服务器端开发、Java应用程序的最终部署环境一般都是Linux
Linux与Windows的区别：
    文件系统不同：
            Linux：目录    Windows：盘符
    外部设备映射不同：
            Linux：挂载点  Windows：盘符
    安全级别不同：
            Linux：高          Windows：低
Linux是基于命令操作的：
     pwd：显示当前工作目录
     ls：查看当前工作目录的内容
     cd：改变当前工作目录
        绝对路径：相对于根目录的位置。以/开头
        相对目录：相对于当前目录的位置
          . ：表示当前目录
         .. ：表示上一级目录

计算机只认识0和1    二进制

**C语言编译运行过程：**
         **.c源文件，经过编译，直接生成可执行文件（0和1）**

**Java编译运行过程：**
        **1： .java源文件，经过编译，生成.class字节码文件**
        **2：JVM（java虚拟机）加载.class并运行.class（0和1）**

**C语言文件-------可执行文件---------操作系统**
**java语言源文件-----字节码文件------JVM  操作系统**

Java开发环境：
       java编译运行过程：
              编译期：.java源文件，经过编译，生成.class
              运行期：JVM加载.class并运行.class
              跨平台，一次编程到处使用
       JVM（Java virtual machines            ）：

​                          java虚拟机   加载.class并运行.class 
​       JRE（Java runtime environment      ）：

​                          java运行环境 除了包含JVM以外还包含运行java程序所必须的环境                                                                                         

​                          JRE=JVM+java系统类库
​       JDK（Java development kit）：

​                           java开发工具包 除了包含JRE以外还包含开发java程序所必须的命令工具
​                           JDK=JRE+编译、运行等等命令工具
​           运行java程序的最小环境为JRE
​           开发java程序的最小环境为JDK
配置环境变量
​      Linux系统：
​        JAVA_HOME:指向jdk的安装目录  JDK装哪里，java_Home就指哪里 

​        CLASSPATH:表示类的搜索路径，一般简写为 （  .  ） 
​        PATH：指向jdk下的bin目录
Eclipse 是目前主流的IDE（集成开发环境）  IBM、开源的、免费的、解压即可使用

开发步骤：

 1.新建一个java项目

 2.新建一个java包

 3.新建一个java类



java代码1.严格区分大小写

​               2.符号必须是英文模式的

​               3.每句话的结束要用;结尾

​               4.println（）：输出并换行

​                  print（）：输出不换行

Linux分两种版本：

​               1.带图形界面的：

​               2.不带图形界面的：

什么 变量？

   就是指代在内存中开辟的存储空间，用于存放运算过程中需要用到的数据。

早期计算机--------算数

现在计算机--------算数

**变量：存数的，代词，指代的就是它所存的那个数**

​          1.声明：变量使用之前必须声明，否则会有编译错误。如果多个变量的*类型一样*，可以在一条语句中声明，中间用逗号分隔。

​                       int a; //声明一个整形变量，名为a

​                       int b，c，d；//声明三个整形变量，名为b，c，d

​          2.命名：变量的命名必须符合Java标识符的规则：

​                         可以由字母、数字、“_"和”$"符组合;

​                         首字母不能以数字开头;

​                         Java大小写敏感，命名变量时需要注意；

​                         不能使用Java保留字、关键字（一些java语言规定好的，有特殊含义的字符）如：int、if、for、break等；  

​                          中文可以作为变量名，但不提倡使用。

​                          驼峰命名法：

​                                     score，myScore，myJavaScore既如果变量的名字由多个单词组成，除第一个单词外，其他单词的首字母大写，其余的子母小写。

​          3.初始化：第一次赋值

​                             1.声明的同时初始化：

​                                      int a=250；//声明整形变量a并赋值为250

​                             2.先声明后初始化：

​                                       int a；//声明整形变量a

​                                       a=250；//给变量a赋值为250

​          4.使用：

​                        必须与数据类型匹配

​                           int a=123.456；//编译错误，数据类型不匹配

​                        对变量的操作就是对它所存的那个数的操作

​                              int  a=5；//声明整型变量a并赋值为5

​                              int   b=a+10；//取出a的值5，加10后，再赋值给b

​                              a=a+10；//取出a的值5，加10后，再赋值给a

​                               system.out.println(a);//输出a的值15

​                                system.out.println("a");//a，原样输出

​                        变量在用之前必须声明并初始化

​                                  system.out.println(m);//编译错误，m未声明

​                                   int m；

​                                   system.out.println(m);//编译错误，m未初始化

​                                    int m=250；

​                                    system.out.println(m);//输出m的值250

​                                   

java中的注释分三种：

​    1.单行注释：//

​    2.多行注释：/*   */

​    3.文档注释：

​    1G=1024M（兆）

​    1M=1024KB（千字节）

​    1KB=1024B（字节）

​    1B=8Bit（位）

Java基本数据类型，分别用于存储整数、浮点数、字符数据和布尔类型数据：

​        整数类型    int类型：最常用的整数类型。一个int类型的变量占用4个字节（32位）-21个多亿到                               

​                                            21个多亿                                          

​                                    1.整数直接量默认为int型，不能超范围，否则会编译错误

​                                    2.两个整数相除，结果还是整数，小数位无条件舍弃

​                                    3.运算时超出范围会发生溢出，溢出是需要避免的

​                                                编译错误（直接量超范围）    溢出（运算时超范围）

​                            long类型：长整型。8字节，很大 

​                                        1.长整型直接量为在数字后加l或L

​                                        2.算数运算时有可能超范围，建议在第一个数字后加l或L

​                                        3. System.currentTimeMillis();用于获取自1970.1.1零时到此时此刻所经历的毫秒数

​                            double类型：浮点型，8个字节，很大

​                                         1.浮点数直接量默认为double型，表示float型需加f或F

​                                         2.double型数据运算时，可能会发生误差

​       精确运算场合不能使用double和float

​                            char类型：字符型，2个字节

​                                           1.Java字符类型采用Unicode字符集编码，Unicode是世界通用的定长字符集，所有的字符都是16位，每个字符（char）都有一个对应的码（int）

​                                           2.字符必须放在单引号中，有且仅有一个

​                                           3.特殊符号需通过\来转义

​                            boolean类型：布尔型，1个字节

​                                          1.只能取值为true或false

​                             byte类型：8位有符号Java原始整数数据类型。范围是-128至127

整数直接量是int类型：所谓整数直接量就是直接写出的整数。

整型数据的除法运算中的取整

dataTypeDemo-------------驼峰命名法

DataTypeDemo-------------帕斯卡命名法（类名）

Java八大基本类型：byte，short，int，long，float，double，char，boolean。

基本类型间的转换：byte，short，int，long，float，double，char。

​                       类型从小到大依次为：byte，short，int，long，float，double。

​                                                                          char可以转换为int

​                                1.两种方式：

​                                   自动类型转换（）：从小类型到大类型

​                                           int a=2；

​                                       long b=a；//自动类型转换（从小到大）

​                                    强制类型转换：从大类型到小类型，有可能会溢出和精度丢失

​                                            int c=（int）b；//强制类型转换（从大到小）

​                                2.两点规则：

​                                     1.   整数直接量可以直接赋值给byte，short，char，但不能超范围

​                                     2.   byte，short，char型变量参与运算时，先一律转为int再运算

Scanner的用法：接受用户输入的数据，也是给变量赋值的一种方式

​          1.在package下：

​                import  java.util.Scanner；

​           2.在main方法中：

​               Scanner scan= new  Scanner（System.in）；

​            3.在第2步之下：

​                 System.out.println（"请输入"）；

​                 int age=scan.nextInt（）；

​                 double  age=scan.nextInt（）；

给变量赋值三种方式：

​          赋值一个固定的值：

​         int  a=5；

​           接受用户输入的一个值：

​          int a=？；

​          系统随机生成一个值：

​            int a=？；

1.运算符：

​        1.算术运算符：+,-,*,/,,%,++,-- 

​                                 1.%：取模/取余，余数为0即位整除

​                                 2.++/--：自增1/自减1，可以在变量钱也可以在变量后

​                                              单独使用时，在前在后无差别

​                                              被使用时，在前在后有差别

​                                             a++的值为a

​                                             ++a的值为a+1

                          package Day03;

public class OperDemo {

	public static void main(String[] args) {
		/*int n=225;
		System.out.println(n%8);*/
		/*int a=3,b=4;
		int c=a++;
		int d=++b;
		System.out.println(c);
		System.out.println(d);
		System.out.println(a);
		System.out.println(b);*/
		int a=9,b=9;
		System.out.println(a++);//9
		System.out.println(a);//10
		System.out.println(++b);//10
		System.out.println(b);//10
	
	}

}

​        2.关系运算符：1.<（小于）,>（大于）,<=（小于等于）,>=（大于等于）,==（等于）,!=（不等于）

​                       2.关系运算的结果为boolean型，关系成立则为true，关系不成立则为false

                               		int a=99,b=200,c=99;
    	boolean d=a>b;
    	System.out.println(d);//false
    	System.out.println(c<=a);//true
    	System.out.println(a<=b);//true
    	System.out.println(a==c);//true
    	System.out.println(a!=c);//false
​        3.逻辑运算符：

​                                 1. &&：短路与（并且），两边都为真则为真，见false则false

        int a=10,b=20,c=10;
    	boolean d=a>b&&c<=b;
    	System.out.println(d);//false
    	System.out.println(a==c&&b<c);//true&&false=false
    	System.out.println(a>b&&a!=c);//false&&false=false
    	System.out.println(b>=a&&c<b);//true&&true=true
​                                          第一个数为false时，发生短路（后面的不执行）

		int a=10,b=20,c=10;
		boolean d=a>b&&a++>10;
		System.out.println(d);//false
		System.out.println(a);//10,短路a不执行++
		boolean e=a<b&&a++>10;
		System.out.println(e);//true
		System.out.println(a);//11,不发生短路执行++
​                                  2. ||：短路或（或者），有一边为真则为真，见true则true

		int a=10,b=20,c=10;
		System.out.println(a>b||c<=b);//false||true=true
		System.out.println(a==c||b<c);//true||false=true
		System.out.println(b>a||b!=c);//true||true=true
		System.out.println(b==c||b<a);//false||false=false
​                                        第一个数为true时，发生短路（后面的不执行）

		int a=10,b=20,c=10;
		boolean d=a<b||a++>10;
		System.out.println(d);//true
		System.out.println(a);//10,发生短路没执行++
		boolean e=a>b||a++>10;
		System.out.println(e);//true
		System.out.println(a);//11,没发生短路执行++
​                                  3. ！：逻辑非（取反），非真则假，非假则真

		int a=10,b=20,c=10;
		boolean d=!(a>b);
		System.out.println(d);//!false=true
		System.out.println(!(c<b));//!true=false
​                                   逻辑运算是建立在关系运算的基础之上的

​                                   逻辑运算的结果也是Boolean型

​        4.赋值运算符：

​                                 简单赋值运算符：=

​                                 扩展赋值运算符：+=，-=，*=，/=，%=扩展赋值运算自动强转

		int a=10;
		a+=20;//a=a+10
		System.out.println(a);//30
		a*=200;//a=a*200
		System.out.println(a);//6000
		a/=5;//a=a/5
		System.out.println(a);//1200
		a-=200;//a=a-200
		System.out.println(a);//1000
		a%=50;//a=a%50
		System.out.println(a);//0
​        5.字符串拼接：‘+’：1.若两边为数字，则做加法运算

		System.out.println(10+20);//30
​                                         2.若有一边字符串，则做字符串拼接

		int age=18;
		System.out.println("age=");//age,原样输出
		System.out.println(age);//18
		System.out.println("age="+age);//age=18
		System.out.println("我的年龄是："+age);
		System.out.println("我今年"+age+"岁了");
		System.out.println(10+20+30+"");//60
		System.out.println(""+10+20+30);//102030
​        6.三目/条件运算符：

​                          语法：

​                                 Boolean？数1：数2

​                          执行过程：

​                                     先计算Boolean表达式：

​                                     若为true，则整个的结果为数1

​                                     若为false，则整个的结果为数2

		int a=99,b=999;
		int max=a>b?a:b;
		System.out.println("max="+max);
​                     条件运算符可以嵌套使用，所谓嵌套是指在三目/条件表达式：“Boolean表达式？表达式1：表达式2”找那个的表达式1或表达式2也是条件/三目表达式。

		int a=-5;
		String b=a>0?"整数大于":(a==0?"0":"小于0");
		System.out.println(b);//小于0
2.分支结构：

​       1.if结构：

​       2.if...else结构：

​       3.if...else if结构：

​       4.switch...case:

闰年的判断公式：

​                   1.能被4整除，并且不能被100整除，

​           或者2.能被400整除