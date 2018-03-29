
### 这是一个根据模块工程生成新项目工程的脚本

#### 主要解决问题：<br>
当项目组需要开发一系列产品时，往往会出现某些功能模块通用的情况，常见的做法是建一个全新的工程，再将这些功能代码一步步添加进去，繁琐费事易出错。这个脚本目的便是避免重复工作，将通用功能模块的代码通过脚本的方式，在新项目生成的时候便已经基本完成，加速开发

#### 目录介绍：<br>
**Template**文件为AndroidStudio项目结构的模板工程<br>
**build**文件为生成脚本
**build_mac**文件为mac系统用的生成脚本，使用方式同build

#### 使用方式：<br>
在shell环境下输入命令：

    ./build ProjectName packageName
    （mac中：  ./build_mac ProjectName packageName）

ProjectName 必须输入，并且该目录下唯一<br>
packageName 字符串以.为分割符，缺省值为com.example.apps<br>
例如：  ./build Test com.example.apps 

#### 扩展：<br>
可在模板工程里面根据实际需要添加功能，但不保证build脚本支持所有的添加，脚本已经做了详细注释，如若不能正常编译，可自行更改脚本<br>
例如：目前在项目中添加了MainActivity.java, appTheme, .gitignore文件，若实际使用项目中不一样，把模板工程里面的文件替换掉就可以了

#### PS:<br>
在更改Template模板工程时，建议导入到AS中修改验证，避免模板工程本身就存在问题


-by UlexZhong

