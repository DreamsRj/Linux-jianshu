# Command : touch

Linux command - Touch
# Touch

该命令用于修改文件的访问时间和最后修改时间。

如果该文件不存在，那么将会创建一个空文件，此时该文件大小为0。 如果指定 `-c` 或 `-h`参数则不会创建空文件。

- 创建空文件

```shell
touch test.sh
ls -l
```

![image-20200430143835495](Linux Command - touch.assets/image-20200430143835495.png)

- 修改文件访问时间和最后修改时间

![image-20200430144316913](Linux Command - touch.assets/image-20200430144316913.png)

文件的访问时间和修改时间均被

![image-20200430144716997](Linux Command - touch.assets/image-20200430144716997.png)