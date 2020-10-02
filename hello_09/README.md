自执行jar包
==========
> scalac -d ./classes src/com/mine/hello/Utils.scala

> scalac -d ./classes -cp ./classes src/Hello.scala

利用manifest.txt
===============
> cp /home/hjh/scala-2.12.12/lib/scala-compiler.jar libs/

> cp /home/hjh/scala-2.12.12/lib/scala-library.jar libs/

> jar cmvf manifest.txt libs/hello.jar -C classes .

> java -jar libs/hello.jar