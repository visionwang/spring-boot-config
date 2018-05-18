#配置服务

此服务基于Spring Cloud Config，为微服务提供配置服务。最终的配置保存在[/config-repo](https://github.com/xiaoyinxi/config-repo)。

###编译打包
```shell
./gradlew clean build
```

###执行测试
```shell
./gradlew clean test
```

###运行配置服务
```shell
java -Dspring.cloud.config.server.git.uri=file:{absolute path of config-repo} -jar pilipa-configserver-1.0.0-SNAPSHOT.jar
```
