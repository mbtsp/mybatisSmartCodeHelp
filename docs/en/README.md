## quick start

### Features

| function points                                                                                                                           | Free version | Paid version |
|-------------------------------------------------------------------------------------------------------------------------------------------|--------------|--------------|
| Support one-click generation of basic information such as configuration DAO SERVICE                                                       | ✔            | ✔            |
| Support the use of common annotations such as @Data                                                                                       | ✔            | ✔            |
| Supports XML attributes to automatically map entities and database table fields                                                           | ✔            | ✔            |
| Supports XML editing auto-suggestion                                                                                                      | ✔            | ✔            |
| Support parameter detection in XML collection                                                                                             | ✔            | ✔            |
| Support Dao method to automatically generate Sql                                                                                          | ✔            | ✔            |
| Support Service to be generated according to different modes                                                                              | ✔            | ✔            |
| Supports @trim entity classes to remove spaces                                                                                            | ✔            | ✔            |
| Support XML sql to automatically generate Dao method~~                                                                                    | ✔            | ✔            |
| Supports custom database tools, the usage method is the same as the one that comes with idea, and it can be used in the community edition | ✔            | ✔            |
| Support TK mapper                                                                                                                         | ✔            | ✔            |
| Database configuration supports oracle                                                                                                    | ✔            | ✔            |
| Support Service mapper method to jump directly to xml file                                                                                | ✔            | ✔            |
| Support multi-table definition one-key generation                                                                                         | ✔            | ✔            |
| Supports dynamic startup of built-in database tools                                                                                       | ✔            | ✔            |
| Detect whether the mapper method is implemented in the xml file, and provide a one-click generation xml method                            | ✔            | ✔            |
| Check whether the return value of mapper is consistent with xml                                                                           | ✔            | ✔            |
| Support internationalization                                                                                                              | ✔            | ✔            |
| Support Mybatis plus3                                                                                                                     | ✘            | ✔            |
| Supports mybatis sql log capture and formatted output                                                                                     | ✘            | ✔            |
| Add field comment display to table configuration UI                                                                                       | ✘            | ✔            |
| Custom database configuration supports one-click import of project database configuration                                                 | ✘            | ✔            |
| Support Xml file #{} parameter to jump to method or actually use class field                                                              | ✘            | ✔            |
| Support xml file Mybatis parameter detection and quick repair                                                                             | ✘            | ✔            |
| Support xml file Mybatis parameter detection                                                                                              | ✘            | ✔            |
| Support mybatis log window to collect project mybatis sql and build it into sql that can be executed directly                             | ✘            | ✔            |
| Support mybatis param parameter jumping                                                                                                   | ✘            | ✔            |
| Support mybatis param parameter refactoring                                                                                               | ✘            | ✔            |
| Support mybatis if test expression refactoring                                                                                            | ✘            | ✔            |
| Support mybatis if test expression jump                                                                                                   | ✘            | ✔            |

## configuration database

- Use IntelliJ IDEA Ultimate version, configure the database information used in the project, you can get built-in advanced tips
- <img alt="image" height="650" src="https://user-images.githubusercontent.com/31949635/161695601-29615d83-dfd0-4587-9e46-11d31169e382.png" width="940"/>
- After configuring the database, the development tool also needs to know which database the SQL statement in the project belongs to, so we also need to configure the dialect corresponding to the database. Different dialects have different prompts and detection information, please choose the correct one.
- <img alt="image" height="650" src="https://user-images.githubusercontent.com/31949635/161696350-f4adcef1-eafb-4b5c-b31f-f6602f2293c7.png" width="940"/>
- .If multiple databases are configured, you need to configure again
- <img alt="image" height="650" src="https://user-images.githubusercontent.com/31949635/161697170-07c348be-f6e0-475c-8fac-e81bda626a5b.png" width="940"/>

## database generation code

### Database generation that comes with the Ultimate version

    - Select the right column Database, click on the table to be generated, if you want to generate multiple tables, select multiple tables at the same time, the 3 position means single table generation, and the 4 position means outright generation
    - ![image](https://user-images.githubusercontent.com/31949635/161704199-322a533b-4daf-48fc-8251-34f7d62fc9fd.png)
    - Configure code generation location
      - 1. The name of the table to be generated
      - 2. Class name after generation
      - 3. Remove the prefix, such as sys_user, if you want to generate a User, you need to enter sys in it
      - 4. When there are multiple modules, you need to choose which module to generate
      - 5. The class to be generated stores the package name path (as long as the package path in the java directory is ok)
      - 6.model store the project directory, eg: D:\workspace\demo\src\main\java
      - 7. The mappper to be generated has a package path (as long as the package path in the java directory is ok)
      - 8. The project directory stored by mapper, eg: D:\workspace\demo\src\main\java
      - 9. Generate the package name corresponding to the mapper xml file (the file name under resource is fine)
      - 10. The mapper xml file stores the project directory, eg: D:\workspace\demo\src\main\resources
      - 11. Simple mode will ignore the method named example, full mode will generate all methods, pure mode will not generate methods, only classes will be generated
      - 12. The name of the package where the service interface is located (as long as the package path in the java directory is ok)
      - 13. The project directory corresponding to the service interface eg: D:\workspace\demo\src\main\java
      - 14. The name of the package where the service implementation class is located (as long as the package path in the java directory is ok)
      - 15. The project directory corresponding to the service implementation class eg: D:\workspace\demo\src\main\java
    - ![](../img.png)
    - Configure database table field information
     - The type of field-level information to be generated can be adjusted
    - ![](../img_1.png)
    - Additional build information configuration
    - ![](../img_2.png)
    - After the configuration is complete, click Finish

### Community edition build

     - Check if the plugin is activated successfully
       - ![](../img_3.png)
       - ![](../img_4.png)
     - After the activation of the plugin is successful, go to the configuration to check whether the database tool with the plugin is enabled, and select to start the built-in database tool
        - File | Settings | Tools | Mybatis Smart Code Help Pro
        - ![](../img_5.png)
     - After checking it, click to restart the idea, at this time there will be a database tool icon on the right
        - ![](../img_6.png)
     - Click + to add the database configuration, you can choose to click the import configuration button to quickly import the database configuration, currently only supports spring boot
        The built-in database configuration ensures that there is a configuration database in the configuration file, and both yml and property files support parsing
        - ![](../img_7.png)
    - Support one-click automatic download of driver files
        - ![](../img_8.png)
    - Support selection of database type and driver version
        - ![](../img_9.png)
    - The subsequent generation operation is the same as the automatic operation of Ultimate.

### code merging

   - Code merging If the Generate Comment is checked in the additional configuration interface, the built-in method of mybatis will be overwritten, and other methods will be merged.
   - If you do not check Generate Comments in the additional configuration interface, it may not be overwritten, and there will be duplicate methods. It is recommended to select Generate Comments. Currently in this plugin
    The plugins provided by their official website that can be merged and covered without checking the generated comments have been used for processing

## method name to generate sql

    ### -  Generate sql based on mapper method name
        - ![](../方法名生成sql.gif)
    ### - Generate sql based on mapper method name (with if test)
        - ![](../方法名生成if-test-sql.gif)
    ### - Generate findAll and selectAll methods
        - ![](../生成findAll和selectALl方法.gif)

## Autocompletion and parameter detection

    ### - xml param autocompletion
        - ![](../param参数补全.gif)
    ### - param check is correct and the type is correct
        -  ![](../param参数检测.gif)
    ### - if test parameter auto-completion
        - ![](../iftest参数补全.gif)
    ### - resultMap property detection and completion
        - ![](../resultMap-property自动补全.gif)
    ### - Collection association auto-completion in resultMap
        - ![](../resultMap-collection自动补全.gif)

## Mybatis log interception

    ### - mybatis log interception, and automatically format sql and fill parameters
        - ![](../mybatis-sql日志拦截,并且填充参数格式化.gif)

## demo

- Plugin
  settings![插件设置](https://user-images.githubusercontent.com/31949635/154419374-81726a9f-d411-424c-9785-aff768b761f2.gif)
- jumps![各种跳转](https://user-images.githubusercontent.com/31949635/154419392-3d6c0f04-111c-49dd-a032-ed5bb8d74d53.gif)
- quick
  fix![快速修复](https://user-images.githubusercontent.com/31949635/154419490-2fcdfbba-f289-4152-a790-22875fc446f5.gif)
- Custom database configuration and one-click import project database
  configuration![配置自定义数据库和导入项目数据库配置](https://user-images.githubusercontent.com/31949635/154419550-070db2d8-b159-4a33-8d93-fec1d2975df6.gif)
- One-click generation of single-table or multi-table
  CURD![生成mybatis UI 配置和操作](https://user-images.githubusercontent.com/31949635/154419631-cc87752d-128b-4bb7-8dc4-ef8ef7ac43a7.gif)
- Mybatis xml parameter one-click completion and parameter
  jump![自动补全和参数跳转](https://user-images.githubusercontent.com/31949635/154419688-4fe6bc14-d991-433a-9018-b7c667968785.gif)
- Detect parameters and hints and
  fixes![动画](https://user-images.githubusercontent.com/31949635/151687957-63e8e956-7738-49e2-a48b-1d6b29bcec18.gif)
- Parameter quick
  fix![参数快速修复](https://user-images.githubusercontent.com/31949635/154419332-ae875668-c780-4fb2-8522-8322bda79beb.gif)
- mybatis sql log
  collection![打印mybatis sql 日志](https://user-images.githubusercontent.com/31949635/154420591-984ee8a8-515f-4cda-bfc9-77d14978f1e6.gif)

## pending function

- ~~Support one-key refactoring of xml parameters, etc.~~
  Reference project

  MybatisX: https://github.com/baomidou/MybatisX

  mybatis-lite: https://plugins.jetbrains.com/plugin/10921-mybatis-lite

  MyBatisCodeHelper-Pro: https://github.com/gejun123456/MyBatisCodeHelper-Pro
