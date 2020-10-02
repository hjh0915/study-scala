单独存放编译后的代码
=================
> scalac -d ./classes src/com/mine/hello/Utils.scala

> scalac -d ./classes -cp ./classes src/Hello.scala

> scala -cp ./classes Hello

> java -cp .:/home/hjh/scala-2.12.12/lib/scala-compiler.jar:/home/hjh/scala-2.12.12/lib/scala-library.jar:./classes Hello

打包
===
> jar cvf libs/utils.jar -C classes com/mine/hello/Utils.class -C classes 'com/mine/hello/Utils$.class'

> scalac -d ./classes -cp libs/utils.jar src/Hello.scala

> jar cvf libs/hello.jar -C classes Hello.class -C classes 'Hello$.class'

> scala -cp libs/utils.jar:libs/hello.jar Hello

> java -cp .:/home/hjh/scala-2.12.12/lib/scala-compiler.jar:/home/hjh/scala-2.12.12/lib/scala-library.jar:./libs/utils.jar:./libs/hello.jar Hello

文件名包含特殊字符
===============
参考资料：https://linux.cn/article-5777-1.html

可以用单引号将其引出