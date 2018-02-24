# Terminal Cheatsheet for Mac (korean)

Original translation by [DaeunGod](https://github.com/DaeunGod)

------------

_대문자는 가독성을 위해 사용되었습니다._  _capslock은 꺼져있어야 합니다._
## 단축키

| Key/Command | 설명 |
| ----------- | ----------- |
| Ctrl + A   | 현재 입력중인 라인의 처음으로 이동합니다.  이 명령어는 대부분의 텍스트 입력에서도 작동합니다.  Netbeans는 예외 입니다. |
| Ctrl + E   | 현재 입력중인 라인의 끝으로 이동합니다. 이 명령어는 대부분의 텍스트 입력에서도 작동합니다. Netbeans는 예외 입니다. |
| Ctrl + Q   | 현재 입력 중인 라인을 지웁니다. |
| Ctrl + L   | 화면을 지웁니다. |
| Cmd + K    | 화면을 지웁니다. |
| Ctrl + U   | 현재 커서 위치에서 입력 라인의 처음까지 잘라냅니다. |
| Ctrl + K   | 현재 커서 위치에서 입력 라인의 끝까지 잘라냅니다. |
| Ctrl + W   | 분리 문자로 공백을 사용하여 현재 커서 위치 이전의 한 단어를 잘라냅니다. |
| Ctrl + Y   | 마지막 잘라내기 명령으로 만들어진 부분을 붙여넣습니다. |
| Ctrl + H   | 백 스페이스와 동일 |
| Ctrl + C   | 현재 터미널에서 실행중인 어떤 것이든 정지합니다. |
| Ctrl + D   | 실행 중인 프로세스가 없으면 현재 쉘을 종료합니다. 또는 EOF를 실행중인 프로세스에 보냅니다. |
| Ctrl + Z   | 실행 중인 프로세스를 중단된 백그라운드 프로세스에 넣습니다. fg명령은 이것을 복원합니다. |
| Ctrl + _   | 마지막 명령을 실행취소합니다. (밑줄을 사용하기 때문에 실제로는 Ctrl + Shift + minus 입니다.) |
| Ctrl + T   | 커서 위치 전에 있는 두 문자를 서로 바꿉니다. |
| Ctrl + F   | 커서를 우측으로 이동합니다. |
| Ctrl + B   | 커서를 좌측으로 이동합니다. |
| Option + →  | 커서를 한 단어 우측으로 이동합니다. |
| Option + ←  | 커서를 한 단어 좌측으로 이동합니다. |
| Esc + T  | 커서 위치 전에 있는 두 단어를 서로 바꿉니다. |
| Tab  | 파일이나 폴더 이름을 자동 완성합니다. |

## 핵심 명령어

| Key/Command | 설명 |
| ----------- | ----------- |
| cd [folder] | 디렉토리를 변경합니다. 예) `cd Documents` |
| cd |  홈 디렉토리 |
| cd ~ |  홈 디렉토리 |
| cd /  | 드라이브의 root |
| cd -  | 이전 디렉토리 |
| ls | 현재 디렉토리의 짧은 목록 |
| ls -l | 현재 디렉토리의 긴 목록 |
| ls -a | 숨겨진 파일이 포함된 목록 |
| ls -lh| 파일 사이즈가 포함된 목록 |
| ls -R | 재귀적으로 모든 폴더의 컨텐츠 표시 |
| sudo [command] | superuser의 보안 권한으로 명령어를 실행합니다. (sudo = Super User DO) |
| open [file] | 파일을 엽니다. ( 더블클릭 한 것처럼 ) |
| top | 현재 동작중인 프로세스를 표시합니다. q를 누르면 표시를 종료합니다. |
| nano [file] | nano 에디터로 파일을 엽니다. |
| vim [file] | vim 에디터를 파일을 엽니다. |
| clear |  화면을 지웁니다. |
| reset |  터미널을 reset합니다. |

## 연쇄 명령어

| Key/Command | 설명 |
| ----------- | ----------- |
| [command-a]; [command-b] | A명령의 성공 여부에 관계없이 A명령 실행 후 B명령을 실행합니다. |
| [command-a] && [command-b] | A명령이 실행 성공하면 B명령을 실행합니다. |
| [command-a] \|\| [command-b] | A명령이 실패하면 B명령을 실행합니다. |
| [command-a] & | A명령을 백그라운드에서 실행합니다. |


## PIPING COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| [command-a] \| [command-b] | Run command A and then pass the result to command B e.g ps auxwww \| grep google |


## COMMAND HISTORY

| Key/Command | Description |
| ----------- | ----------- |
| history n |  Shows the stuff typed – add a number to limit the last n items |
| Ctrl + r  | Interactively search through previously typed commands |
| ![value] |  Execute the last command typed that starts with ‘value’ |
| ![value]:p |  Print to the console the last command typed that starts with ‘value’ |
| !! |  Execute the last command typed |
| !!:p |  Print to the console the last command typed |

## FILE MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| touch [file] |   Create a new file |
| pwd | Full path to working directory |
| . |  Current folder, e.g. `ls .` |
| .. | Parent/enclosing directory, e.g. `ls ..` |
| ls -l .. | Long listing of parent directory |
| cd ../../ | Move 2 levels up |
| cat | Concatenate to screen |
| rm [file] |  Remove a file, e.g. `rm data.tmp` |
| rm -i [file] | Remove with confirmation |
| rm -r [dir] | Remove a directory and contents |
| rm -f [file] | Force removal without confirmation |
| cp [file] [newfile] | Copy file to file |
| cp [file] [dir] | Copy file to directory |
| mv [file] [new filename] |  Move/Rename, e.g. `mv file1.ad /tmp` |
| pbcopy < [file] | Copies file contents to clipboard |
| pbpaste | Paste clipboard contents |
| pbpaste > [file] | Paste clipboard contents into file, `pbpaste > paste-test.txt` |

## DIRECTORY MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| mkdir [dir] | Create new directory |
| mkdir -p [dir]/[dir] |  Create nested directories |
| rmdir [dir] | Remove directory ( only operates on empty directories ) |
| rm -R [dir] | Remove directory and contents |
| less [file]|  Output file content delivered in screensize chunks |
| [command] > [file] |  Push output to file, keep in mind it will get overwritten |
| [command] >> [file] | Append output to existing file |
| [command] < [file] |  Tell command to read content from a file |

## SEARCH

| Key/Command | Description |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Search for files, e.g. `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Search for all lines that contain the pattern, e.g. `grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | Recursively search in all files in specified directory for all lines that contain the pattern |
| grep -v [search_pattern] [file] | Search for all lines that do NOT contain the pattern |
| grep -i [search_pattern] [file] | Search for all lines that contain the case-insensitive pattern |
| mdfind [search_pattern] | Spotlight search for files (names, content, other metadata), e.g. `mdfind skateboard` |
| mdfind -onlyin [dir] -name [pattern] | Spotlight search for files named like pattern in the given directory |

## HELP

| Key/Command | Description |
| ----------- | ----------- |
| [command] -h |  Offers help |
| [command] --help | Offers help |
| info [command] | Offers help |
| man [command] |  Show the help manual for [command] |
| whatis [command] | Gives a one-line description of [command] |
| apropos [search-pattern] | Searches for command with keywords in description |
