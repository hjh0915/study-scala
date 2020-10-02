执行测试代码
==========
参考资料:
http://www.scalatest.org/quick_start

> scalac Utils.scala

> scalac -cp .:./libs/scalatest_2.12-3.1.1.jar:./libs/scalactic_2.12-3.1.1.jar TestUtils.scala

> scala -cp .:./libs/scalatest_2.12-3.1.1.jar:./libs/scalactic_2.12-3.1.1.jar org.scalatest.run TestUtils

执行
===
> scalac -cp . Hello.scala

> scala -cp . Hello

> java -cp .:/home/hjh/scala-2.12.12/lib/scala-compiler.jar:/home/hjh/scala-2.12.12/lib/scala-library.jar Hello