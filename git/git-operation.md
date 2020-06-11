# Git 常用操作



## 设置中文文件名称被编码为unicode

默认情况下,中文名称的文件显示将错乱:

![image-20200611233846921](git-operation.assets/image-20200611233846921.png)

设置属性:

```shell
git config --global core.quotepath false
```

设置之后,显示正常

![image-20200611233946574](git-operation.assets/image-20200611233946574.png)