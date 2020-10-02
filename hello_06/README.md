包的使用
=======
特殊之处在于：可以不写目录但是直接用package
在Utils.scala 增加
``` scala
package com.mine.hello
```
> scalac Utils.scala

在HelloWorld.scala 增加
``` scala
import com.mine.hello._
```
> scalac -cp . Hello.scala

> scala -cp . Hello

> java -cp .:/home/hjh/scala-2.12.12/lib/scala-compiler.jar:/home/hjh/scala-2.12.12/lib/scala-library.jar Hello

执行代码之后
==========
如果是以包的形式的话，那么编译之后会生成目录，并且编译后的文件会自动放置设置的目录下