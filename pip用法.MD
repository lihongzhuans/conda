1、列出当前python环境已经安装的第三方模块列表

`pip freeze `或 `pip list`

2、导出当前python环境已经安装的第三方模块列表

将当前环境已经安装的第三方模块导出到桌面的requirements.txt文件

pip freeze > /Desktop/requirements.txt

*3、在线安装第三方模块或者通过requirements.txt进行模块安装*

*普通用法：pip install modelName* 

*安装指定版本模块: pip install modelName==0.0.1(不指定版本则默认安装最新版本)*

如果同时安装的模块较多建议通过requirements.txt来将模块罗列出来进行安装

也可以通过命令来同时安装多个模块：pip install modelA modelB

4、pip工具更新

python -m pip install --upgrade pip 或者 pip install -U pip

5、更新指定模块

pip install -U modelName 或者

 **pip install modeName --upgrade**

如果有多个需要进行升级的模块可通过requirements.txt文件来进行，将文件中模块版本的==替换为>=

#### 6、第三方模块卸载

pip uninstall modelName

## 安装指定模块或版本

* `conda install package-name`
* `conda install package-name==version`

7、显示已经安装的某模块信息

Pip show modelName

8、验证已经安装的python模块是否具有依赖关系

pip check(个人很少用到)

9、列出所有已经安装的未更新的模块列表

pip list -o

10、显示模块安装所在目录

pip show -f modelName

11、在线搜索模块

pip_search modelName

有可能会报错，

![](https://pic2.zhimg.com/80/v2-1f1e503ab98f5ab091bd278a2f9edf59_720w.webp)

如果显示上述异常则是search功能被禁用了，需执行pip install pip_search安装此模块。

12、pip离线下载模块

pip download modelName -d 目录地址 或

pip download -d 目录地址 -r requirements.txt

13、pip安装本地文件(所谓的离线安装)

Cd 模块所在目录:

Pip install *.whl 或 python setup.py install
