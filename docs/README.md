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
 - 使用IntelliJ IDEA Ultimate 版本的，配置好项目中使用的数据库信息,可以得到内置的高级提示
 - <img alt="image" height="650" src="https://user-images.githubusercontent.com/31949635/161695601-29615d83-dfd0-4587-9e46-11d31169e382.png" width="940"/>
 - 配置好数据库之后,开发工具还需要知道项目里面sql语句是哪个数据库的,所以我们还要配置下数据库对应的方言,方言不同，提示和检测的信息不同，请选择正确。
 - <img alt="image" height="650" src="https://user-images.githubusercontent.com/31949635/161696350-f4adcef1-eafb-4b5c-b31f-f6602f2293c7.png" width="940"/>
 - .如果配置了多个数据库,还需要再次配置
 - <img alt="image" height="650" src="https://user-images.githubusercontent.com/31949635/161697170-07c348be-f6e0-475c-8fac-e81bda626a5b.png" width="940"/>
 
## 数据库生成代码
  ### Ultimate 版本自带的Database 生成
    - 选择右则栏位Database,点击要生成的表,如果想要多表生成，同时选择多张表,3 位置表示单表生成, 4位置表示夺标生成
    - ![image](https://user-images.githubusercontent.com/31949635/161704199-322a533b-4daf-48fc-8251-34f7d62fc9fd.png)
    - 配置代码生成位置
      - 1.要生成的表名 
      - 2.生成之后类名称 
      - 3.去除前缀,比如sys_user,想要生成User 就要在这里面输入sys   
      - 4.多模块的时候,要选择生成在哪个module中
      - 5.要生成的类存放包名路径(只要java目录下的包路径就可以)
      - 6.model存放工程目录,eg：D:\workspace\demo\src\main\java
      - 7.要生成的mappper存在包路径(只要java目录下的包路径就可以)
      - 8.mapper存放的工程目录，eg：D:\workspace\demo\src\main\java
      - 9.生成mapper xml 文件对应的包名(resource下面的文件名称就可以了)
      - 10.mapper xml文件存放工程目录，eg：D:\workspace\demo\src\main\resources
      - 11.简易模式会忽略example命名的方法,完整模式则会生成全部的方法,纯净模式则不会生成方法,只会生成类
      - 12.service接口所在的包名称(只要java目录下的包路径就可以)
      - 13.service接口对应的工程目录eg：D:\workspace\demo\src\main\java
      - 14.service实现类所在的包名称(只要java目录下的包路径就可以)
      - 15.service实现类对应的工程目录eg：D:\workspace\demo\src\main\java
    - ![img.png](img.png)
    - 配置数据库表字段信息
     - 可以调整要生成的字段级别信息,类型
    - ![img_1.png](img_1.png)
    - 额外生成信息配置
    - ![img_2.png](img_2.png)
    - 配置好了之后,直接点击完成
  ### 社区版生成
     - 先查看插件是否激活成功
       - ![img_3.png](img_3.png)
       - ![img_4.png](img_4.png)
     - 激活插件成功之后,还要去配置中查看插件带的数据库工具是否开启,选择勾选启动内置数据库工具
        - File | Settings | Tools | Mybatis Smart Code Help Pro
        - ![img_5.png](img_5.png)
     - 勾选之后,点击重起idea,这个时候在右则就有数据库工具图标出来了
        - ![img_6.png](img_6.png)
     - 点击+来添加数据库配置,可以选择点击导入配置按钮来快速导入数据库的配置,目前只支持spring boot 
        自带的数据库配置,确保配置文件中有配置数据库,yml 和property文件的都支持解析
        - ![img_7.png](img_7.png)
    - 支持一键自动下载驱动文件
        - ![img_8.png](img_8.png)
    - 支持选择数据库类型和驱动版本
        - ![img_9.png](img_9.png)
    - 后续生成操作就和Ultimate自动的一样操作就可以了
  ### 代码合并方式
    -  代码合并如果在额外配置界面勾选了生成注释,则mybatis 内置的方法会进行覆盖,其他的方法合并的方式处理
    -  如果在额外配置界面没有勾选生成注释,则可能不会进行覆盖,会出现重复方法,建议勾选生成注释，当前本插件中
      已经使用了他们官网提供的不勾选生成注释也可以进行合并覆盖的插件进行处理
## 方法名生成sql
    ### -  根据mapper方法名称生成sql
        - ![](方法名生成sql.gif)
    ### - 根据mapper方法名称生成sql(带if test)
        - ![](方法名生成if test sql.gif)
    ### - 生成findAll和selectAll方法
        - ![](生成findAll和selectALl方法.gif)
## 自动补全和参数检测
    ### - xml param 自动补全
        
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
