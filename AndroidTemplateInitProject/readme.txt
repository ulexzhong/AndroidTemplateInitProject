
这是一个根据模块工程生成新项目工程的脚本

Template文件为AndroidStudio项目结构的模板工程
build文件为生成脚本

使用方式：
在shell环境下输入命令： ./build yourProjectName

可在模板工程里面根据实际需要添加功能，但不保证build脚本支持所有的添加，脚本已经做了详细注释，若不能正常编译，可自行更改脚本
例如：目前在项目中添加了appTheme, .gitignore文件，若实际使用项目中不一样，把模板工程里面的文件替换掉就可以了

在更改Template模板工程时，建议导入到AS中修改验证，避免模板工程本身就存在问题

-by UlexZhong