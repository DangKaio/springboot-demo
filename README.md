# springboot-demo
##SpringBoot学习

1.Spring Boot的基础结构共三个文件（具体路径根据用户生成项目时填写的Group所有差异）
    src/main/java下的程序入口：DemoApplication
    src/main/resources下的配置文件：application.properties
    src/test/下的测试入口：DemoApplicationTests

##引入web模块

初始pom.xml:
    spring-boot-starter：核心模块，包括自动配置支持、日志和YAML
    spring-boot-starter-test：测试模块，包括JUnit、Hamcrest、Mockito
2. 引入web模块,需添加spring-boot-starter-web模块    
    maven仓库地址：https://mvnrepository.com/
    编写服务HelloController
    创建package命名为com.demo.controller（根据实际情况修改）
    创建HelloController类
    启动主程序，打开浏览器访问http://localhost:8080/hello，可以看到页面输出Hello World
  
3.编写单元测试
  编写一个简单的单元测试来模拟http请求
  使用MockServletContext来构建一个空的WebApplicationContext，这样我们创建的HelloController就可以
  在@Before函数中创建并传递到MockMvcBuilders.standaloneSetup（）函数中。
  
4.增加文件夹
    config:配置文件夹
    controller:控制器
    dao:操作数据库
    model: 数据实体
    service: 服务层
    
    mybatis-config.xml:mybatis配置文件夹
    
    先创建model中的实体类，在编写dao层操作数据库，编写service，在编写controll