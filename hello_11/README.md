整体打包
=======
修改build.gradle
```groovy
plugins {
    .....

    id "com.github.johnrengelman.shadow" version "5.2.0"
}

jar {
    manifest {
        attributes 'Main-Class': 'hello_10.Hello'
    }
}
```

执行
===
> gradle build

> gradle shadowJar

> java -jar build/libs/hello_11-all.jar