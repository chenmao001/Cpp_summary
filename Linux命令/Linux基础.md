# Linux基础

### 关机

```bash
shutdown -h +时间
reboot
```

### 目录介绍

```bash
etc lib bin dev usr
```

### 目录相关命令

```bash
ls -al
cd
mkdir
rmdir 只能删除空目录 -p递归删除
cp + 源文件 + 目标目录
mv 移动
rm -r-f
```

### 文件属性

```bash
chgrp   修改所属组
chown   修改所有者
chmod 770 filename 更改文件权限
```

### 文件内容查看

```bash
cat 从第一行显示文件
tac 从最后一行显示文件
nl 同时显示行号
more   /字符串  查找
less
head -n n控制显示多少行
tail
```

### 硬链接和软连接

```bash
ln souce dest
ln -s source dest
touch
echo 输出字符串，也可以定向到文件到文件中 echo "It is a test" > myfile
```

### 磁盘管理

```bash
df 列出文件系统整体的磁盘使用量 -h易于读的显示方式
du 列出当前文件的磁盘使用情况 -a -h
mount 外部设备 /mnt/目录名  挂载外部设备到mnt
unmount -f 【挂载位置】强制卸载
```

### 进程管理

```bash
ps -a 显示当前终端运行的所有进程 -u 以用户信息的形式显示 -x 显示所有进程，不以终端区分
ps -aux | grep mysql
ps -ef | grep 可以查看到父进程的进程号
grep(global search regular expression(RE) and print out the line,全面搜索正则表达式并把行打印出来)
grep [-acinv] [--color=auto] '搜寻字符串' filename
选项与参数：
-a ：将 binary 文件以 text 文件的方式搜寻数据
-c ：计算找到 '搜寻字符串' 的次数
-i ：忽略大小写的不同，所以大小写视为相同
-n ：顺便输出行号
-v ：反向选择，亦即显示出没有 '搜寻字符串' 内容的那一行！
--color=auto ：可以将找到的关键词部分加上颜色的显示喔！
```

