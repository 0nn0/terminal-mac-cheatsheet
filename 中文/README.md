# Terminal Cheatsheet for Mac ( 基本 )
Original translation by [kavlez](https://github.com/kavlez)  
Modified translation by [kestory](https://github.com/kestory)

------------

## 快捷键

| 按键/命令 | 描述 |
| -------- | ---- |
| Ctrl + A | 移动光标至行首，也适用于大多数文本编辑器 |
| Ctrl + E | 移动光标至行尾，也适用于大多数文本编辑器 |
| Ctrl + Q | 清除当前行中的所有内容 |
| Ctrl + L | 清屏 |
| Command + K | 清屏 |
| Ctrl + U | 剪切光标前的所有字符 |
| Ctrl + K | 剪切光标后的所有字符 |
| Ctrl + W | 剪切光标前的内容，直到遇到为止 |
| Ctrl + Y | 粘贴上一次剪切的字符 |
| Ctrl + H | 与退格键相同 |
| Ctrl + C | 终止当前执行的进程 |
| Ctrl + D | 当没有进程在执行时退出当前终端，如果当前有进程就发送 `EOF` 命令给当前进程 |
| Ctrl + Z | 将执行中的任何东西放入后台进程。fg 可以将其恢复。 |
| Ctrl + _ | 撤销最后一条命令（因为是下划线，所以实际上是 `Ctrl + Shift + _`）|
| Ctrl + T | 将光标前的两个文字进行互换 |
| Ctrl + F | 将将光标向前移动一个字符 |
| Ctrl + B | 将将光标向后移动一个字符 |
| Option + → | 光标向前移动一个单词 |
| Option + ← | 光标向后移动一个单词 |
| Esc + T | 将光标前的两个单词进行互换 |
| Tab | 自动补全文件或文件夹的名称 |


## 核心命令

| 按键/命令 | 描述 |
| -------- | ---- |
| cd [folder] | 切换目录，例如 `cd Documents`|
| cd | Home目录 |
| cd ~ | Home目录|
| cd / | 根目录 |
| cd - | 上一个目录 |
| ls | 文件列表 |
| ls -l | 文件详细列表 |
| ls -a | 列出隐藏文件 |
| ls -lh | 详细文件列表中文件大小以更友好的形式列出 |
| ls -R | 递归显示文件夹中的内容 |
| sudo [command] | 以超级用户身份执行命令 |
| open [file] | 打开文件 ( 相当于双击一个文件 ) |
| top | 显示运行中的进程，按q终止 |
| nano [file] | 使用 nano 打开编辑 |
| vim	[file] | 使用 vim 打开编辑 |
| clear | 清屏 |
| reset | 重置终端显示 |

## 命令链

| Key/Command | Description |
| ----------- | ----------- |
| [command-a]; [command-b] |不管命令 a 是否执行成功，执行完命令 a 后再执行命令 b |
| [command-a] && [command-b] | 如果命令 a 执行成功就执行命令 b |
| [command-a] \|\| [command-b] | 如果命令 a 执行失败就执行命令 b|
| [command-a] & | 在后台执行命令 a |


## 命令管道

| Key/Command | Description |
| ----------- | ----------- |
| [command-a] \| [command-b] | 运行命令 a，然后将结果给命令 b，例如 `ps auxwww | grep google` |


## 管道命令

| 按键/命令 | 描述 |
| -------- | ---- |
| history n | 列出最近执行过的 n 条命令 |
| ctrl-r | 检索之前执行过的命令 |
| ![value] | 执行最近以 `value` 开始的命令 |
| ![value]:p | 显示最近以 `value` 开始的命令 |
| !! | 执行最后一次执行的命令 |
| !!:p |  显示最后一次执行的命令 |

## 命令历史

| 按键/命令 | 描述 |
| -------- | ---- |
| history n |  列出最近执行过的n条命令 |
| ctrl-r |  交互式检索之前执行过的命令 |
| ![value] |  执行最近以'value'开始的命令 |
| ![value]:p |  将最近以'value'开始的命令打印到终端 |
| !! |  执行上一条命令 |
| !!:p |  将上一条命令打印到终端 |

## 文件管理

| 按键/命令 | 描述 |
| -------- | ---- |
| touch [file] | 创建一个新文件 |
| pwd | 显示当前工作目录 |
| . |  当前目录, 例如 `ls .` |
| .. | 上级目录, 例如 `ls ..` |
| ls -l .. |  上级目录的文件详细列表 |
| cd ../../| 向上移动两个层级 |
| cat | 连接或打印文件到屏幕上 |
| rm [file] | 移除文件, 例如 `rm data.tmp` |
| rm -i [file] | 移除时出现确认提示 |
| rm -r [dir] | 移除文件及内容 |
| rm -f [file] | 强制移除 |
| cp [file] [newfile] | 复制文件 |
| cp [file] [dir] | 复制文件到指定目录 |
| mv [file] [new filename] | 移动/重命名, 例如 `mv file1.ad /tmp`|
| pbcopy < [file] | 把内容复制到剪切板中 |
| pbpaste | 粘贴剪切板中的内容 |
| pbpaste > [file] | 把剪切板中的内容复制到文件里 `pbpaste > paste-test.txt` |

## 目录管理

| 按键/命令 | 描述 |
| -------- | ---- |
| mkdir [dir] | 创建新目录 |
| mkdir -p [dir]/[dir] | 创建子目录 |
| rmdir [dir] | 移除目录 ( 仅限目录下没有内容时 ) |
| rm -R [dir] | 移除目录及内容 |
| less [file]|  根据当前终端窗口大小来输出文件内容 |
| [command] > [file] |  将命令输出的内容覆盖到文件里 |
| [command] >> [file] | 将命令输出的内容附加到文件里 |
| [command] < [file] |  告诉命令从文件中读取内容 |
 

## 搜索

| Key/Command | Description |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | 搜索文件, 例如 `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | 搜索文件中含有关键字的所有行, e.g. `grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | 递归搜索目录的所有文件中包含该关键字的所有行 |
| grep -v [search_pattern] [file] | 搜索文件中不含有关键字的所有行 |
| grep -i [search_pattern] [file] | 搜索文件中含有关键字（不区分大小写）的所有行 |
| mdfind [search_pattern] | 用 Spotlight 搜搜文件 (搜索范围包涵名字、内容、其他文件数据), 例如 `mdfind skateboard` |
| mdfind -onlyin [dir] -name [pattern] | 用 Spotlight 搜索制定目录中名字包涵关键字的文件 |


## 帮助

| 按键/命令 | 描述 |
| -------- | ---- |
| [command] -h | 显示帮助信息 |
| [command] --help | 显示帮助信息 |
| info [command] | 提供帮助 |
| man [command] | 显示指定命令的帮助信息 |
| whatis [command] | 显示指定命令的简述 |
| apropos [search-pattern] | 使用关键字搜索描述内容 |
