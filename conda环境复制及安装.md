### * conda导出已有环境，环境会被保存在environment.yaml文件中

```
 conda env export > environment.yaml
```

### * 当我们想再次创建该环境，或根据别人提供的.yaml文件复现环境时，就可以通过下面的命令来复现安装环境了。根据环境文件进行复制

```
conda env create -f environment.yaml
```

### * **查看已有的虚拟环境，选择你要切换到的虚拟环境**

```
conda info --envs
```

**
    或者**

```
conda env list
```

### * **在命令行中切换到想要的虚拟环境，我这里切换到自己的环境**

```
conda activate myownerenv_name
```

### * 将当前环境已经安装的第三方模块导出到桌面的requirements.txt文件

```
pip freeze > /Desktop/requirements.txt
```

### conda升级

```
conda update conda
```
