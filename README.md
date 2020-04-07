#项目说明
消息队列主要用来处理耗时的业务逻辑或者为了提高响应速率，并且不必要实时处理的功能的情况下；或者为了削峰；当然还可以解耦。这里可以归属为第一种情况下的应用场景。
springboot + rabbitmq 保证消息100%投递成功并被消费

#应用场景
主要是针对特别重要的消息，必须成功投递、成功消费的情况

#打包部署
例如： mvn clean package -Dmaven.test.skip=true
##测试环境启动
java -jar app.jar --spring.profiles.active=test

##正式环境启动
java -jar app.jar --spring.profiles.active=prod

#项目配置说明

##运行环境
- **jdk**
 ```1.8以上```
 
- **mysql**
 ```5.7以上```

- **redis**
 ```3.0以上```

- **rabbitmq**
 ```3.6以上```