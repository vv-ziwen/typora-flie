## 设置与配置

### 1、显示工具栏

> 标注1：View–>Toolbar
> 标注2：View–>Tool Buttons

### 2、设置鼠标悬浮提示

> File–>settings–>Editor–>General–>勾选Show quick documentation on mouse move

### 3、显示方法分隔符

> File–>settings–>Editor–>General–>Appearance–>勾选Show method separators

### 4、自动导包

> File–>settings–>Editor–>general–>Auto Import–>勾选Add unambiguous imports on the fly

### 5、单行显示多个Tabs

> File–>settings–>Editor–>General -->Editor Tabs–>去掉√

### 6、设置字体大小

> File–>settings–>Editor–>Font–>Size

### 7、生成缺少文件

> IDEA中的`.iml`文件是项目标识文件，缺少了这个文件，IDEA就无法识别项目。跟Eclipse的`.project`文件性质是一样的。并且这些文件不同的设备上的内容也会有差异，所以我们在管理项目的时候，`.project和.iml文件都需要忽略掉`。
>
> - 生成`.ipr`文件: `mvn idea:project`
> - 生成`.iws`文件: `mvn idea:workspace`
> - 生成`.iml`文件: `mvn idea:module`

### 8、热部署

> 

### 9、Maven

> **1：分析剔除无用的jar引用**
>
> 使用如下命令：
>
> ```mvn
> mvn dependency:analyze
> ```
>
> 会输出如下的日志：
>
> - Used undeclared dependencies found
>
>   这个是指某些依赖的包在代码中有用到它的代码，但是它并不是直接的依赖（就是说没有在pom中直接声明），是通过引入传递下来的包。
>
> - Unused declared dependencies found
>
>   这个是指我们在pom中声明了依赖，但是在实际代码中并没有用到这个包！也就是多余的包。 这个时候我们就可以把这个依赖从pom中剔除。
>
> **2：高效找出全部未被使用的代码**
>
> Analyze -> Run Inspection by Name -> 输入 undeclared



## 代码模板



## 断点调试



## 整合Git



## 整合Maven

