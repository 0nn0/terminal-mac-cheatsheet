### 快捷鍵

| 按鍵/命令 | 解釋 |
| ----------- | ----------- |
| Ctrl + A   | 移動游標到行首，適用大部分文字編輯器 |
| Ctrl + E   | 移動游標到行末，適用大部分文字編輯器 |
| Ctrl + L   | 清空版面 |
| Cmd + K    | 清空版面 |
| Ctrl + U   | 清除整行文字 |
| Ctrl + K   | 清除游標後的所有文字 |
| Ctrl + W   | 清除游標前的所有文字 |
| Ctrl + Y   | 貼上前一次剪下的任何東西 |
| Ctrl + H   | 跟backspace一樣 |
| Ctrl + C   | 停止任何執行中的東西，同時清除整行文字 |
| Ctrl + D   | 退出目前終端機，或送`EOF`給執行中的程式 |
| Ctrl + Z   | 把正在執行的作業移到後台執行，`fg`可以將其恢復 |
| Ctrl + _   | 取消上一個命令 (底線，所以其實是 Ctrl + Shift + 減號) |
| Ctrl + T   | 將游標前兩個字互換 |
| Ctrl + F   | 將游標往前移一格 |
| Ctrl + B   | 將游標往後移一格 |
| Option + →  | 將移飆往前移一個詞 |
| Option + ←  | 將游標往後移一個詞 |
| Esc + T  | 將游標前兩個詞互換 |
| Esc + Backspace | 刪除前一個用空白隔開的詞 |
| Tab  | 自動補齊命令 |

### 核心命令

| 按鍵/命令 | 解釋 |
| ----------- | ----------- |
| cd [folder] | 改變目前目錄位置 例如：`cd Documents` |
| cd |  回家目錄 |
| cd ~ |  回家目錄|
| cd /  | 到根目錄 |
| cd -  | 回上一層目錄 |
| ls | 列出檔案名 |
| ls -l | 列出檔案名和資訊 |
| ls -a | 列出所有檔案，包括用`.`開頭的隱藏檔案 |
| ls -lh| 列出檔名和資料大小 |
| ls -R | 用遞迴的方式列出所有檔案，包括所有資料夾以下的資料夾和檔案 |
| sudo [command] | 用系統管理員身分執行命令 |
| open [file] | 打開檔案 (就像對一個檔案點兩下) |
| top | 顯示所以執行中的程式 (按`q`離開) |
| nano [file] | 用nano文字編輯器打開檔案 |
| vim [file] | 用vim文字編輯器打開檔案 |
| clear | 清空版面 |
| reset | 重新整理終端機 |

### 命令鏈

| 按鍵/命令 | 解釋 |
| ----------- | ----------- |
| [command-a]; [command-b] | 不管A有沒有成功，執行A完執行B  |
| [command-a] && [command-b] | 執行A成功後，執行B |
| [command-a] \|\| [command-b] | A不成功才執行B |
| [command-a] & | 在後台執行A |


### 管道命令

| 按鍵/命令 | 解釋 |
| ----------- | ----------- |
| [command-a] \| [command-b] | 執行A並把A的結果傳給B 例如：`ps auxwww \| grep google` |


### 李史紀錄

| 按鍵/命令 | 解釋 |
| ----------- | ----------- |
| history n |  列出最近執行的n條命令 |
| Ctrl + r  | 互動式搜尋執行過的命令 |
| ![value]  |  執行最近以"value"開頭的命令 |
| ![value]:p|  顯示最近以"value"開頭的命令 |
| !! |  執行上一個命令 |
| !!:p |  顯示上一個命令 |

### 檔案管理

| Key/Command | Description |
| ----------- | ----------- |
| touch [file] |   新增一個叫做"file"的檔案 |
| pwd | 顯示目前路徑 |
| . |  代表目前路徑 例如：`ls .` |
| .. | 代表上一層目錄 例如：`ls ..` |
| ls -l .. | 列出上一層目錄的檔案和資訊 |
| cd ../../ | 移動到前兩層目錄|
| cat | 預覽檔案 |
| rm [file] |  刪除檔案 例如 `rm data.tmp` |
| rm -i [file] | 經過確認後再刪除文件 |
| rm -r [dir] | 刪除資料夾和裡面的所有東西 |
| rm -f [file] | 強制刪除檔案 |
| cp [file] [dir] | 複製文件到新資料夾 |
| mv [file] [new filename] | 重新命名文件 例如 `mv file1.ad /tmp` |
| pbcopy < [file] | 複製內容到剪貼板 |
| pbpaste | 貼上剪貼板的內容 |
| pbpaste > [file] | 將剪貼板的內容貼到檔案中 例如：`pbpaste > paste-test.txt` |

### 資料夾管理

| Key/Command | Description |
| ----------- | ----------- |
| mkdir [dir] | 創建新資料夾 |
| mkdir -p [dir]/[dir] |  創建子資料夾 |
| rmdir [dir] | 刪除資料夾，只會作用在空資料夾 |
| rm -R [dir] | 刪除資料夾和其內容 |
| less [file] | 根據目前視窗大小顯示檔案內容 |
| [command] > [file] |  將命令的輸出輸入到檔案中 (原本的內容會被覆蓋) |
| [command] >> [file] | 將命令的輸出接在目標檔案的內容後面 |
| [command] < [file] |  告訴命令讀取檔案內容 |

### 搜尋

| Key/Command | Description |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | 尋找檔案 例如：`find /Users -name "file.txt"` |
| grep [search_pattern] [file] | 尋找檔案中包含關鍵字的每一行 例如：`grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | 尋找資料夾中包含關鍵字的每一行 |
| grep -v [search_pattern] [file] | 尋找資料夾不中包含關鍵字的每一行 |
| grep -i [search_pattern] [file] | 尋找檔案中包含關鍵字的每一行(不區分大小寫) |
| mdfind [search_pattern] | 用Spotlight搜尋關鍵字(搜尋內容包括文件、內容等) 例如：`mdfind skateboard` |
| mdfind -onlyin [dir] -name [pattern] | 用Spotlight在指定資料夾中搜尋關鍵字 |

### 幫助

| Key/Command | Description |
| ----------- | ----------- |
| [command] -h | 顯示提示 |
| [command] --help | 顯示提示 |
| info [command] | 顯示提示 |
| man [command] |  顯示此命令得說明書 |
| whatis [command] | 顯示一個一行的提示 |
| apropos [search-pattern] | 用關鍵字尋找命令 |

