# Terminal Cheatsheet for Mac ( 基本 )
Original translation by [kavlez](https://github.com/kavlez)

------------

## 快捷键

| 按键/命令 | 描述 |
| -------- | ---- |
| Ctrl + A | 移动光标至行首 |
| Ctrl + E | 移动光标至行尾 |
| Ctrl + Q | 清除当前行 |
| Ctrl + L | 清屏（相当于 clear 命令） |
| Cmd + K | 清屏（无法上翻看历史了） |
| Ctrl + U | 删除光标之前到行首的字符 |
| Ctrl + K | 删除光标之前到行尾的字符 |
| Ctrl + W | 以空白符为分隔向左删一个单词 |
| Ctrl + Y | 粘贴最后一次被删除的内容 |
| Ctrl + H | 等同于退格符 |
| Ctrl + R | 根据用户输入查找相关历史命令 |
| Ctrl + C | 终止当前执行 |
| Ctrl + D | 没有进程运行时退出当前shell，否则向当前运行进程发送EOF |
| Ctrl + Z | 将任何执行中的东西放入后台进程。fg可以将其恢复。 |
| Ctrl + _ | 撤销上次命令（是下划线，所以其实是 Ctrl + Shift + minus） |
| Ctrl + T | 将光标前的两个字符进行互换 |
| Ctrl + F | 将光标向前移动一个字符 |
| Ctrl + B | 将光标向后移动一个字符 |
| Option + → | 将光标向前移动一个单词 |
| Option + ← | 将光标向后移动一个单词 |
| Esc + T | 将光标前的两个单词进行互换 |
| Tab | 自动补全文件或文件夹的名称 |


## 核心命令

| 按键/命令 | 描述 |
| -------- | ---- |
| cd [folder] | 切换目录 |
| cd | 主目录 |
| cd ~ | 主目录 |
| cd / | 磁盘根目录 |
| ls | 简洁文件列表 |
| ls -l | 详细文件列表 |
| ls -a | 列出隐藏文件 |
| ls -lh | 详细文件列表中文件大小以更友好的形式列出 |
| ls -R | 递归显示文件夹中的内容 |
| sudo [command] | 以超级用户身份执行命令 |
| open [file] | 打开文件 ( 相当于双击一个文件 ) |
| top | 显示运行中的进程，按q终止 |
| nano [file] | 用nano打开编辑 |
| vim	[file] | 用vim打开编辑 |
| clear | 清屏 |
| reset | 重置终端显示 |

## 链接命令

| 按键/命令 | 描述 |
| -------- | ---- |
| [command-a]; [command-b] | 顺序执行命令A和命令B，不管A是否执行成功 |
| [command-a] && [command-b] | 命令A执行成功后执行命令B |
| [command-a] \|\| [command-b] | 命令A执行失败后执行命令B |
| [command-a] & | 在后台执行命令A |


## 管道命令

| Key/Command | Description |
| ----------- | ----------- |
| [command-a] \| [command-b] | Run command A and then pass the result to command B e.g ps auxwww \| grep google |


## 命令历史

| 按键/命令 | 描述 |
| -------- | ---- |
| history n | 列出最近执行过的n条命令 |
| ctrl-r | 检索之前执行过的命令 |
| ![value] | 执行最近以'value'开始的命令 |
| !! | 执行最近执行过的命令 |


## 文件管理

| 按键/命令 | 描述 |
| -------- | ---- |
| touch [file] | 创建一个新文件 |
| pwd | 显示当前工作目录 |
| .. | 上级目录, 例如. |
| | 'ls -l ..' 	= 上级目录的文件详细列表 |
| | 'cd ../../' = 向上移动两个层级 |
| . | 当前目录 |
| cat | 连接 |
| rm [file] | 移除文件, 例如 rm [file] [file] |
| rm -i [file] | 移除时出现确认提示 |
| rm -r [dir] | 移除文件及内容 |
| rm -f [file] | 强制移除 |
| cp [file] [newfile] | 复制文件 |
| cp [file] [dir] | 复制文件到指定目录 |
| mv [file] [new filename] | 移动/重命名, 例如 mv -v [file] [dir] |


## 目录管理

| 按键/命令 | 描述 |
| -------- | ---- |
| mkdir [dir] | 创建新目录 |
| mkdir -p [dir]/[dir] | 创建子目录 |
| rmdir [dir] | 移除目录 ( 仅限目录下没有内容时 ) |
| rm -R [dir] | 移除目录及内容 |



##

| 按键/命令 | 描述 |
| -------- | ---- |
| more | 按当前窗口大小输出内容 |
| > [file] | 输出至指定文件, 注意文件将会覆盖 |
| >> [file] | 在制定文件的末尾附加内容 |
| < | 从文件中读取内容 |


## 帮助

| 按键/命令 | 描述 |
| -------- | ---- |
| [command] -h | 显示帮助信息 |
| [command] --help | 显示帮助信息 |
| [command] help | 显示帮助信息 |
| reset | 重置当前终端 |
| man [command] | 显示指定命令的帮助信息 |
| whatis [command] | 显示指定命令的简述 |
