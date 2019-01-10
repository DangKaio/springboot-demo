# springboot-demo
SpringBoot学习

1.Spring Boot的基础结构共三个文件（具体路径根据用户生成项目时填写的Group所有差异）
src/main/java下的程序入口：DemoApplication
src/main/resources下的配置文件：application.properties
src/test/下的测试入口：DemoApplicationTests

初始pom.xml:
spring-boot-starter：核心模块，包括自动配置支持、日志和YAML
spring-boot-starter-test：测试模块，包括JUnit、Hamcrest、Mockito
2.引入web模块,需添加spring-boot-starter-web模块    https://mvnrepository.com/
  编写服务HelloController，启动成功