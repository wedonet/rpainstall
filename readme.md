# Rpa安装软件

## 运行环境

- Win10,64位
- Office 2013以上版本（Work, Excel, Powerpoint)

## 安装建议

下面的软件，建议装在D盘，统一建一个文件夹Rpa，Rpa用到的软件都装在这个文件夹下面，便于管理和备份。


## 编辑器

- VsCode
安装包：VSCodeUserSetup-x64-1.59.0.exe
安装时选创建桌面快捷方式，添加到PATH(重启后生效)。
VsCode装Python插件。

- Atom
AtomSetup-x64.exe

## 装Sogo输入法

## 装Python

安装包： python-3.9.6-amd64.

路径选择 d：/rpa/python

安装时选择 'Add Python 3.9 to Path'，其它默认认装。

验证安装是否成功，在CMD中执行
```
python -V
```

显示出 'Python Python 3.9.6' 版本信息，表示安装成功。


## Chrome浏览器

安装包： 92.0.4515.107_chrome64_stable_windows_installer.exe  （ver 92.0.4515.107）

安装后禁用Chrome自动更新,（禁用方法 ：windows服务中禁用Chrome更新，禁用任务计划），改名更新程序文件名

```
更新服务：
Google 更新服务 (gupdate)
Google 更新服务 (gupdatem)
Google Chrome Elevation Service (GoogleChromeElevationService)

任务计划：
GoogleUpdateTaskMachineCore
GoogleUpdateTaskMachineUA

GoogleUpdate.exe 默认路径
C:\Program Files (x86)\Google\Update\GoogleUpdate.exe
```

## Chrome驱动

安装包： chromedriver_win32.zip

解压 chromedriver.exe到python安装目录下。

## MicrosoftEdge浏览器

版本： 93.0.961.38
安装包： MicrosoftEdgeSetup.exe

禁用edge自动更新，在服务中关掉Microsoft ...edge相关服务。

## MicrosoftEdge浏览器驱动

edgedriver_win64.zip

解压msedgedriver.exe到python目录下。

## IE驱动

IEDriverServer_x64_3.150.2.zip

解压到python目录下。

## Python插件

### Selenium

```
pip install Selenium
```

验证是否能处理网页,运行 hairongmail/baidu.py, 显示success即表示安装成功。

```
python baidu.py
```

验证是否能处理excel,在c盘根目录下建Temp文件夹，运行excel.py,显示success表示安装成功。

```
python excel.py
```

### PyWin32

pywin32-301.win32-py3.9.exe

会自动找到python按装路径，默认安装即可。

## Inspect

windows控件识别软件。

安装包： inspect.exe

免安装软件，发送快捷方式到桌面即可。

## Sqlite

数据库


安装包： sqlite-dll-win32-x86-3360000.zip


## sqlitestudio-3.3.3

数据库管理工具

安装包： sqlite目录下的压缩文件。

创建文件夹 d:\rpa\sqlite，并在此文件夹下解压上面目录下的两个压缩文件，将得到 sqlite3.def、sqlite3.dll 和 sqlite3.exe 文件。

添加 d:\rpa\sqlite 到 PATH 环境变量，最后在命令提示符下，使用 sqlite3 命令，将显示如下结果。

C:\>sqlite3
SQLite version 3.7.15.2 2013-01-09 11:53:05
Enter ".help" for instructions
Enter SQL statements terminated with a ";"
sqlite>

## sqlitestudio-3.3.3.zip

sqlite管理工具，解压后发送.exe文件到桌面即可。

## Putty

ssh客户端

安装包：putty-64bit-0.76-installer.msi

默认安装即可。

## Git

版本管理工具

安装包 Git-2.33.0.2-64-bit.exe

路径选择d:rpa/git,其它默认安装。

安装后运行菜单 help->showsshkey->生成sshkey

验证方法：在文件夹右键，有git选项

##  pandoc-2.14.2-windows-x86_64.msi

转换Atom为PDF等文档格式。

路径d:\rpa\pandoc, 其它默认安装
