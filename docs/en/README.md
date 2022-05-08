## quick start

### Features

| function points                                                                                                                           | Free version | Paid version | Plugin version |
|-------------------------------------------------------------------------------------------------------------------------------------------|--------------|--------------|----------------|
| Support one-click generation of basic information such as configuration DAO SERVICE                                                       | ✔            | ✔            | 2022.1.1+      |
| Support the use of common annotations such as @Data                                                                                       | ✔            | ✔            | 2022.1.1+      |
| Supports XML attributes to automatically map entities and database table fields                                                           | ✔            | ✔            | 2022.1.1+      |
| Supports XML editing auto-suggestion                                                                                                      | ✔            | ✔            | 2022.1.1+      |
| Support parameter detection in XML collection                                                                                             | ✔            | ✔            | 2022.1.1+      |
| Support Dao method to automatically generate Sql                                                                                          | ✔            | ✔            | 2022.1.1+      |
| Support Service to be generated according to different modes                                                                              | ✔            | ✔            | 2022.1.1+      |
| Supports @trim entity classes to remove spaces                                                                                            | ✔            | ✔            | 2022.1.1+      |
| Support XML sql to automatically generate Dao method~~                                                                                    | ✔            | ✔            | 2022.1.1+      |
| Supports custom database tools, the usage method is the same as the one that comes with idea, and it can be used in the community edition | ✔            | ✔            | 2022.1.1+      |
| Support TK mapper                                                                                                                         | ✔            | ✔            | 2022.1.1+      |
| Database configuration supports oracle                                                                                                    | ✔            | ✔            | 2022.1.1+      |
| Support Service mapper method to jump directly to xml file                                                                                | ✔            | ✔            | 2022.1.1+      |
| Support multi-table definition one-key generation                                                                                         | ✔            | ✔            | 2022.1.1+      |
| Supports dynamic startup of built-in database tools                                                                                       | ✔            | ✔            | 2022.1.1+      |
| Detect whether the mapper method is implemented in the xml file, and provide a one-click generation xml method                            | ✔            | ✔            | 2022.1.1+      |
| Check whether the return value of mapper is consistent with xml                                                                           | ✔            | ✔            | 2022.1.1+      |
| Support internationalization                                                                                                              | ✔            | ✔            | 2022.1.1+      |
| Support Mybatis plus3                                                                                                                     | ✘            | ✔            | 2022.1.1+      |
| Supports mybatis sql log capture and formatted output                                                                                     | ✘            | ✔            | 2022.1.1+      |
| Add field comment display to table configuration UI                                                                                       | ✘            | ✔            | 2022.1.1+      |
| Custom database configuration supports one-click import of project database configuration                                                 | ✘            | ✔            | 2022.1.1+      |
| Support Xml file #{} parameter to jump to method or actually use class field                                                              | ✘            | ✔            | 2022.1.1+      |
| Support xml file Mybatis parameter detection and quick repair                                                                             | ✘            | ✔            | 2022.1.1+      |
| Support xml file Mybatis parameter detection                                                                                              | ✘            | ✔            | 2022.1.1+      |
| Support mybatis log window to collect project mybatis sql and build it into sql that can be executed directly                             | ✘            | ✔            | 2022.1.1+      |
| Support mybatis param parameter jumping                                                                                                   | ✘            | ✔            | 2022.1.5+      |
| Support mybatis param parameter refactoring                                                                                               | ✘            | ✔            | 2022.1.5+      |
| Support mybatis if test expression refactoring                                                                                            | ✘            | ✔            | 2022.1.5+      |
| Support mybatis if test expression jump                                                                                                   | ✘            | ✔            | 2022.1.5+      |
| Support manual selection of mybatis sql log to convert to sql and execute                                                                 | ✘            | ✔            | 2022.2.0+      |
| Support plug-in database to directly execute sql script                                                                                   | ✘            | ✔            | 2022.2.0+      |
| Support connection database property field configuration                                                                                  | ✘            | ✔            | 2022.2.0+      |
| Support dynamic plugin icon configuration                                                                                                 | ✘            | ✔            | 2022.2.0+      |
## configure plugin
### configuration database

- Use IntelliJ IDEA Ultimate version, configure the database information used in the project, you can get built-in advanced tips
- ![image](https://user-images.githubusercontent.com/31949635/161695601-29615d83-dfd0-4587-9e46-11d31169e382.png)
- After configuring the database, the development tool also needs to know which database the SQL statement in the project belongs to, so we also need to configure the dialect corresponding to the database. Different dialects have different prompts and detection information, please choose the correct one.
- ![image](https://user-images.githubusercontent.com/31949635/161696350-f4adcef1-eafb-4b5c-b31f-f6602f2293c7.png)
- .If multiple databases are configured, you need to configure again
- ![image](https://user-images.githubusercontent.com/31949635/161697170-07c348be-f6e0-475c-8fac-e81bda626a5b.png)
### Configure the plugin icon
- ![](../ScreenShot/配置插件图标.gif)
## database

  ### Database generation that comes with the Ultimate version
- Select the right column Database, click on the table to be generated, if you want to generate multiple tables, select multiple tables at the same time, the 3 position means single table generation, and the 4 position means outright generation
- Configure code generation location
  - 1. The name of the table to be generated
  - 2. Class name after generation
  - 3. Remove the prefix, such as sys_user, if you want to generate a User, you need to enter sys in it
  - 4. When there are multiple modules, you need to choose which module to generate
  - 5. The class to be generated stores the package name path (as long as the package path in the java directory is ok)
  - 6. model store the project directory, eg: D:\workspace\demo\src\main\java
  - 7. The mappper to be generated has a package path (as long as the package path in the java directory is ok)
  - 8. The project directory stored by mapper, eg: D:\workspace\demo\src\main\java
  - 9. Generate the package name corresponding to the mapper xml file (the file name under resource is fine)
  - 10. The mapper xml file stores the project directory, eg: D:\workspace\demo\src\main\resources
  - 11. Simple mode will ignore the method named example, full mode will generate all methods, pure mode will not generate methods, only classes will be generated
  - 12. The name of the package where the service interface is located (as long as the package path in the java directory is ok)
  - 13. The project directory corresponding to the service interface eg: D:\workspace\demo\src\main\java
  - 14. The name of the package where the service implementation class is located (as long as the package path in the java directory is ok)
  - 15. The project directory corresponding to the service implementation class eg: D:\workspace\demo\src\main\java
  - ![](../ScreenShot/img.png)
- Configure database table field information
  - The type of field-level information to be generated can be adjusted
   - ![](../ScreenShot/img_1.png)
- Additional build information configuration
- ![](../ScreenShot/img_2.png)
- After the configuration is complete, click Finish
  ### Community edition build
     - Check if the plugin is activated successfully
       - ![](../ScreenShot/img_3.png)
       - ![](../ScreenShot/img_4.png)
     - After the activation of the plugin is successful, go to the configuration to check whether the database tool with the plugin is enabled, and select to start the built-in database tool
        - File | Settings | Tools | Mybatis Smart Code Help Pro | Project Setting
        - ![](../ScreenShot/img_5.png)
     - After checking it, click to restart the idea, at this time there will be a database tool icon on the right
        - ![](../ScreenShot/img_6.png)
     - Click + to add the database configuration, you can choose to click the import configuration button to quickly import the database configuration, currently only supports spring boot
        The built-in database configuration ensures that there is a configuration database in the configuration file, and both yml and property files support parsing
        - ![](../ScreenShot/img_7.png)
    - Support one-click automatic download of driver files
        - ![](../ScreenShot/img_8.png)
    - Support selection of database type and driver version
        - ![](../ScreenShot/img_9.png)
    - The subsequent generation operation is the same as the automatic operation of Ultimate.
  ### code merging
    - Code merging If Generate Comments is checked in the additional configuration interface, the built-in methods of mybatis will be overwritten, and other methods will be merged.
    - If you do not check Generate Comments in the additional configuration interface, it may not be overwritten, and there will be duplicate methods. It is recommended to select Generate Comments. Currently in this plugin
    The plugins provided by their official website that can be merged and covered without checking the generated comments have been used for processing
  ### One-click generation of the xml file of mybatis generator
    - ![](../ScreenShot/一键生成mybatis-generator-config.xml.gif)
  ### Configure database connection properties
    - ![](../ScreenShot/配置插件数据库连接属性.gif)
  ### Quick query table data
    - Double-click the table name to quickly query table data
    - ![](../ScreenShot/快速查询表数据.gif)
  ### sql file executes sql statement
    - ![](../ScreenShot/sql文件执行sql语句.gif)

## method name to generate sql
  ### Generate sql based on mapper method name
  ![](../ScreenShot/方法名生成sql.gif)
  ###  Generate sql based on mapper method name (with if test)
  ![](../ScreenShot/方法名生成if-test-sql.gif)
  ###  Generate findAll and selectAll methods
  ![](../ScreenShot/生成findAll和selectALl方法.gif)
  ###  Generate insertAll and insertBatch methods
  ![](../ScreenShot/生成insertAll和insertBatch方法.gif)
  ###  Generate updateBatch and updateBatchSeletive methods
  ![](../ScreenShot/生成updateBatch和updateBatchSeletive方法.gif)
## Autocompletion and parameter detection
  ###  xml param autocompletion
  ![](../ScreenShot/param参数补全.gif)
  ###  param check is correct and the type is correct
  ![](../ScreenShot/param参数检测.gif)
  ###  if test parameter auto-completion
  ![](../ScreenShot/iftest参数补全.gif)
  ###  resultMap property detection and completion
  ![](../ScreenShot/resultMap-property自动补全.gif)
  ###  Collection association auto-completion in resultMap
  ![](../ScreenShot/resultMap-collection自动补全.gif)
## Mybatis log interception
  ###  mybatis log interception, and automatically format sql and fill parameters
  ![](../ScreenShot/mybatis-sql-log.gif)
  ###  Mybatis sql log Manual selection, one-click conversion to sql statement, and you can directly execute to see the statement results
  - This function needs to configure the database configuration of the idea flagship version of the Database Tool or the database configuration that comes with the plugin
  - If both the Database Tool database and the plugin's own database are configured, use the Database Tool first
  - Database configuration, and directly use the Database Tool console.sql function to execute sql
  - If only the database that comes with the plug-in is configured, use the built-in interface of the plug-in for data display
  - ![](../ScreenShot/选择mybatis-sql日志,转成sql语句并执行.gif)
  ### Mybatis sql log interception configuration
  - ![](../ScreenShot/mybatis日志拦截配置.gif)

## Reference project

  MybatisX: https://github.com/baomidou/MybatisX

  mybatis-lite: https://plugins.jetbrains.com/plugin/10921-mybatis-lite

  MyBatisCodeHelper-Pro: https://github.com/gejun123456/MyBatisCodeHelper-Pro
