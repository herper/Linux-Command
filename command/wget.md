# wget

**wget** 命令用来从指定的URL下载文件。wget非常稳定，它在带宽很窄的情况下和不稳定网络中有很强的适应性，如果是由于网络的原因下载失败，wget会不断的尝试，直到整个文件下载完毕。如果是服务器打断下载过程，它会再次联到服务器上从停止的地方继续下载。这对从那些限定了链接时间的服务器上下载大文件非常有用。

## 使用说明

### 语法

```
$ wget[选项][参数]
```

### 选项

```
-a<日志文件>：在指定的日志文件中记录资料的执行过程； 
-A<后缀名>：指定要下载文件的后缀名，多个后缀名之间使用逗号进行分隔； 
-b：进行后台的方式运行wget； 
-B<连接地址>：设置参考的连接地址的基地地址； 
-c：继续执行上次终端的任务； 
-C<标志>：设置服务器数据块功能标志on为激活，off为关闭，默认值为on；
-d：调试模式运行指令； 
-D<域名列表>：设置顺着的域名列表，域名之间用“，”分隔； 
-e<指令>：作为文件“.wgetrc”中的一部分执行指定的指令； 
-h：显示指令帮助信息； 
-i<文件>：从指定文件获取要下载的URL地址； 
-l<目录列表>：设置顺着的目录列表，多个目录用“，”分隔； 
-L：仅顺着关联的连接； 
-r：递归下载方式； 
-nc：文件存在时，下载文件不覆盖原有文件； 
-nv：下载时只显示更新和出错信息，不显示指令的详细执行过程； 
-q：不显示指令执行过程； 
-nh：不查询主机名称； 
-v：显示详细执行过程； 
-V：显示版本信息； 
--passive-ftp：使用被动模式PASV连接FTP服务器； 
--follow-ftp：从HTML文件中下载FTP连接文件。

```

### 参数
```
URL：下载指定的URL地址。
```

**基本使用**

```
$ wget -[选项][参数]
```

**实例演示**

```
[root@linux-command ~]# wget https://wordpress.org/latest.tar.gz
```

**- 选项使用**

```
$ wget -
```

## 温馨提示

**wget** 命令。