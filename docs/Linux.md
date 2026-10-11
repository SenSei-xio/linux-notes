# Linux 命令笔记

pwd：显示当前所在目录

ls：显示当前目录有什么

ls -a：显示隐藏文件夹

cd：切换目录

    cd ..：回上级
    
    cd ~：回到自己家目录

mkdir：新建文件夹

    mkdir -p：可以一次新建很多层文件夹

echo：打印文字

    echo "文字" > 文件名：将文字写入

cat：看文件里的内容

cp：复制文件

mv：移动文件

    mv：在同目录里用就是改名。

rm：删除文件

    rm -r：删除目录   

man ls：打开说明书

q：退出

grep 关键词 文件：在文件里搜索关键词

​	grep -n 关键词 文件：-n显示行号，grep = 在文件中找到包含关键词的行

find：按条件找文件

​	find . -name "*.txt"：列出当前目录下所有的.txt文件

​	find . -type d：只列出目录，按照find找文件，.表示从当前目录往下找

chmod：改权限

​	chmod 600 fruits.txt：语法，数字规则：`r=4`、`w=2`、`x=1`，三位分别是"自己 / 同组 / 其他人

ps：看自己正在跑的进程，只有前三个

​	ps aux：列出所有进程

top：看谁在吃资源

df：看磁盘剩多少空间

ss：看端口和链接

tar：打包/解包

​	tar -czvf docs1.tar.gz docs1

​	**tar** = 打包（`-c`）/ 解包（`-x`）、`-z` 走 gzip、`-v` 显示过程、`-f` 指定文件名

curl：发送网络请求

​	curl -I https://www.baidu.com

systemctl管服务

systemctl is-system-running/ `running`
systemctl list-units --type=service | head -15/ 含义：**systemctl** = 查看 / 启动 / 停止系统服务

