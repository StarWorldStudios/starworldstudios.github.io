# 帮助 - StarWorld Script
> 作者：StarWorld 、 小邓学编程

## 什么是 SWS
StarWorld Script，简称SWS，这是一个由 StarWorld 开发的解释性语言，语法和Batch相似，使代码变得更简单
## 开始使用
> 如果您已经看到这个教程了，那么您应该已经拥有SWS的主程序了吧？
 如果您没有主程序（starworldscript.exe），请重新安装程序。

### 开始配置
为了方便使用，这里我们将会把此程序添加到【环境变量】
>1. 打开【环境变量】配置页面
>2. 选择【PATH】
>3. 将starworldstudioscript.exe的路径添加到PATH中，一路确定。

### 编写HelloWorld程序
1. 随便打开一个目录
2. 【新建】->【文本文档】
3. 将文档重命名为【HelloWorld.sws】
4. 使用【文本编辑器】打开文件
5. 输入以下代码:
```bash
echo StarWorldScript v{version}
echo HelloWorld!
```
6. 在此目录打开【终端命令行】
7. 在【终端命令行】中输入以下代码：
```bash
starworldscript HelloWorld.sws
```
至此，您成功完成了您的第一个HelloWorld程序！

## 错误处理
SWS有两种错误
- 解释器错误
- 代码错误
### 解释器错误
这种错误一般是由解释器漏洞或者代码编写不当导致的，出现这种错误时，解释器会输出`An internal fatal error occurred while executing the command`并退出。
#### 解决方案
- 检查您的代码是否有错误；- 
- 联系开发者以资讯反馈。
### 代码错误
这种错误是由代码编写不当导致的，出现这种情况时，解释器会输出以下代码并跳过出错的代码继续执行。
```python
    StarWorldScript Error Analysis:
       Error in line  错误内容存在行 :
          Error code: " 错误的代码 "
             Error type: " 错误的类型：错误描述"
```
#### 解决方案
- 检查出错的代码

## 代码
> 1.1.3

### echo
- 输出内容(可使用【PlaceholderAPI】变量: `{version} {br} {path} {ctime} {unix_timestamp} {random}` )
- `echo 内容`

### sha1
 - 输出Sha1文本
 - `sha1 内容`
 
### dir
- 查看当前目录文件
- `dir`

### type
- 读取文件内容
- `type 文件`

### purl(Parse URL)
- 读取网页内容（headers参数可不填）
```json
purl {"type":"请求类型","url":"请求URL","data":{"发送数据键名":"发送数据键值"},"headers":{"设置请求头类型":"设置请求头内容"}}
```

### cd
- 转到目录（可使用相对路径和绝对路径）
- `cd 目录`
- `.`：当前目录；`..`: 上级目录


### \#
- `#` 作为StarWorldScript的注释
- `#` 后面的代码是不会被解析器解析的



关于：[StarWorldComunity](https://starworld.itcraft.tk)