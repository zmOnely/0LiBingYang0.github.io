# Day1
### 1.Linux操作系统结构
	用户
	应用层
	Shell层    可以写Shell命令
	内核层 	   为硬件解析命令
	硬件

home文件夹是存放普通用户的的文件夹
d rwx    r-x      r-x  分成三段查看 d代表文件夹 其余代表权限(r读,w写,x执行)
  root  用户组    用户

bin 目录下放可执行文件
etc 放的是环境文件
usr 装东西存放的目录
home 每创建一个用户就会在home文件夹下面创建相应的文件夹
hostname 查看主机名
hostname s 修改用户名为s一次性修改重启后恢复

### 用户切换
	su 从普通用户切换到root
	exit 从root切换到普通用户

## 系统的重启与关机

### 重启
	reboot  重启
	shutdown -r now 立刻重启(root用户使用)
	shutdown -r 10 过10分钟自动重启(root用户使用)
	shutdown -r 20:35 在时间为20:35时候重启(root用户使用)
	shutdown -c 取消重启
### 关机
	halt 立刻关机
	poweroff 立刻关机
	shutdown -h now 立刻关机(root用户使用)
	shutdown -h 10   10分钟后自动关机
### 编辑文件
	vi /etc/hostname 永久修改主机名
	vi 编辑文件 进入文件后 i 进行编辑
	退出时 esc + : + q(退出不保存)/q!(强制退出不保存)/wq(保存并退出)


ping命令 测试网络连通性 格式  ping+ip或端口号

ifconfig 查看所有活动网络接口的信息
yum install net-tools /y   安装网络相关的配置  /y  在碰到选择是自动执行y

service firewalld status 查看防火墙状态
systemctl stop firewalld 临时关闭防火墙
systemctl disable firewalld  禁止开机启动防火墙

Linux文本中 #开头的代表注释

Linux命令的通用命令格式
命令字 [选项] [参数]
选项:用于调节命令的具体功能
参数：命令操作的对象，如文件、目录名等

pwd:查看当前所在目录的全路径
cd:切换工作目录  格式:cd [目录位置]
ls -R:递归查询
ls -a:查看所有文件包括隐藏文件
ls -A:查看除了隐藏文件外的所有文件

mkdir:创建文件夹
mkdir -p:同时创建多层文件夹

du:统计目录和文件占用空间的情况
du -s:统计每个参数所占空间大小
touch:创建文件
> :文件名 创建文件与touch功能相同
echo:向文件里面写内容


cp:复制文件或目录  格式  cp [选项] 源文件或目录 目标文件或目录
-r:复制整个目录树
-p:保持源文件的属性不变
-f:强制覆盖同名文件或目录
-i:需要覆盖时会提醒

rm:移除  常用 rm -rf 直接删除

mv:移动 原路径相当于改名字
