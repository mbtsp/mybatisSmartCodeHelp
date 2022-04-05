## 快速开始
### 功能
| 功能点                                              | 免费版本 | 收费版本 |
|--------------------------------------------------|------|------|
| 支持配置DAO SERVICE 等基本信息的一键生成                       | ✔    | ✔    |
| 支持@Data 等常见注解的使用                                 | ✔    | ✔    |
| 支持XML 属性自动映射实体和数据库表字段                            | ✔    | ✔    |
| 支持XML 编辑自动提示                                     | ✔    | ✔    |
| 支持XML collection中的 参数检测                          | ✔    | ✔    |
| 支持Dao方法自动生成Sql                                   | ✔    | ✔    |
| 支持Service根据不同模式生成                                | ✔    | ✔    |
| 支持@trim 实体类去除空格                                  | ✔    | ✔    |
| 支持XML sql自动生成Dao方法~~                             | ✔    | ✔    |
| 支持自定义数据库工具,使用方法和idea 自带的一样,满足在社区版中使用             | ✔    | ✔    |
| 支持TK mapper                                      | ✔    | ✔    |
| 数据库配置支持oracle                                    | ✔    | ✔    |
| 支持Service mapper 方法直接跳转到xml文件                    | ✔    | ✔    |
| 支持多表单独定义一键生成                                     | ✔    | ✔    |
| 支持动态启动内置数据库工具                                    | ✔    | ✔    |
| 检测mapper方法是否在xml文件中实现,并且提供一键生成xml方法              | ✔    | ✔    |
| 检测mapper返回值是否和xml一致                              | ✔    | ✔    |
| 支持国际化                                            | ✔    | ✔    |
| 支持Mybatis plus3                                  | ✘    | ✔    |
| 支持mybatis sql 日志的抓取和格式化输出                        | ✘    | ✔    |
| 表配置UI增加字段注释展示                                    | ✘    | ✔    |
| 自定义数据库配置支持一键导入项目数据库配置                            | ✘    | ✔    |
| 支持Xml文件#{}参数跳转到方法或者实际使用类字段                       | ✘    | ✔    |
| 支持xml 文件Mybatis 参数检测和快速修复                        | ✘    | ✔    |
| 支持xml 文件Mybatis 参数检测                             | ✘    | ✔    |
| 支持mybatis log 窗口统一收集项目mybatis sql并且构建成可以直接执行的sql | ✘    | ✔    |
| 支持mybatis param参数跳转                              | ✘    | ✔    |
| 支持mybatis param 参数重构                             | ✘    | ✔    |
| 支持mybatis if test 表达式 重构                         | ✘    | ✔    |
| 支持mybatis if test 表达式 跳转                         | ✘    | ✔    |

## 配置数据库
 1.使用IntelliJ IDEA Ultimate 版本的，配置好项目中使用的数据库信息,可以得到内置的高级提示
![image](https://user-images.githubusercontent.com/31949635/161695601-29615d83-dfd0-4587-9e46-11d31169e382.png)
 2.配置好数据库之后,开发工具还需要知道项目里面sql语句是哪个数据库的,所以我们还要配置下数据库对应的方言,方言不同，提示和检测的信息不同，请选择正确。
 ![image](https://user-images.githubusercontent.com/31949635/161696350-f4adcef1-eafb-4b5c-b31f-f6602f2293c7.png)
 3.如果配置了多个数据库,还需要再次配置
 ![image](https://user-images.githubusercontent.com/31949635/161697170-07c348be-f6e0-475c-8fac-e81bda626a5b.png)
## 数据库生成代码
  ### Ultimate 版本自带的Database 生成
    1.选择右则栏位Database,点击要生成的表,如果想要多表生成，同时选择多张表,3 位置表示单表生成, 4位置表示夺标生成
    ![image](https://user-images.githubusercontent.com/31949635/161704199-322a533b-4daf-48fc-8251-34f7d62fc9fd.png)
    2.
## demo
- Plugin settings![插件设置](https://user-images.githubusercontent.com/31949635/154419374-81726a9f-d411-424c-9785-aff768b761f2.gif)
- jumps![各种跳转](https://user-images.githubusercontent.com/31949635/154419392-3d6c0f04-111c-49dd-a032-ed5bb8d74d53.gif)
- quick fix![快速修复](https://user-images.githubusercontent.com/31949635/154419490-2fcdfbba-f289-4152-a790-22875fc446f5.gif)
- Custom database configuration and one-click import project database configuration![配置自定义数据库和导入项目数据库配置](https://user-images.githubusercontent.com/31949635/154419550-070db2d8-b159-4a33-8d93-fec1d2975df6.gif)
- One-click generation of single-table or multi-table CURD![生成mybatis UI 配置和操作](https://user-images.githubusercontent.com/31949635/154419631-cc87752d-128b-4bb7-8dc4-ef8ef7ac43a7.gif)
- Mybatis xml parameter one-click completion and parameter jump![自动补全和参数跳转](https://user-images.githubusercontent.com/31949635/154419688-4fe6bc14-d991-433a-9018-b7c667968785.gif)
- Detect parameters and hints and fixes![动画](https://user-images.githubusercontent.com/31949635/151687957-63e8e956-7738-49e2-a48b-1d6b29bcec18.gif)
- Parameter quick fix![参数快速修复](https://user-images.githubusercontent.com/31949635/154419332-ae875668-c780-4fb2-8522-8322bda79beb.gif)
- mybatis sql log collection![打印mybatis sql 日志](https://user-images.githubusercontent.com/31949635/154420591-984ee8a8-515f-4cda-bfc9-77d14978f1e6.gif)

## pending function
  - ~~Support one-key refactoring of xml parameters, etc.~~
Reference project

    MybatisX: https://github.com/baomidou/MybatisX
   
    mybatis-lite: https://plugins.jetbrains.com/plugin/10921-mybatis-lite
   
    MyBatisCodeHelper-Pro: https://github.com/gejun123456/MyBatisCodeHelper-Pro
