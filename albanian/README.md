
# Përmbledhje e komandave të Terminalit për Mac (Bazat)

------------

_Shkronjat janë në versionin kapital për t'u lexuar më lehtë._  _Butoni Capslock duhet të jetë i fikur._


## SHKURTIME

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| Ctrl + A   | Go to the beginning of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + E   | Go to the end of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + L   | Clears the Screen |
| Cmd + K    | Clears the Screen |
| Ctrl + U   | Cut everything backwards to beginning of line |
| Ctrl + K   | Cut everything forward to end of line |
| Ctrl + W   | Cut one word backwards using white space as delimiter |
| Ctrl + Y   | Paste whatever was cut by the last cut command |
| Ctrl + H   | Same as backspace |
| Ctrl + C   | Kill whatever you are running.  Also clears everything on current line |
| Ctrl + D   | Exit the current shell when no process is running, or send EOF to a the running process |
| Ctrl + Z   | Puts whatever you are running into a suspended background process. fg restores it |
| Ctrl + _   | Undo the last command. (Underscore.  So it's actually Ctrl + Shift + minus) |
| Ctrl + T   | Swap the last two characters before the cursor |
| Ctrl + F   | Move cursor one character forward |
| Ctrl + B   | Move cursor one character backward |
| Option + →  | Move cursor one word forward |
| Option + ←  | Move cursor one word backward |
| Esc + T  | Swap the last two words before the cursor |
| Esc + Backspace | Cut one word backwards using none alphabetic characters as delimiters |
| Tab  | Auto-complete files and folder names |


## KOMANDAT THEMELORE

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| cd [folder] | Change directory e.g. `cd Documents` |
| cd |  Home directory |
| cd ~ |  Home directory |
| cd /  | Root of drive |
| cd -  | Previous directory |
| ls | Short listing |
| ls -l | Long listing |
| ls -a | Listing incl. hidden files |
| ls -lh| Long listing with Human readable file sizes |
| ls -R | Entire content of folder recursively |
| sudo [command] | Run command with the security privileges of the superuser (Super User DO) |
| open [file] | Opens a file ( as if you double clicked it ) |
| top | Displays active processes. Press q to quit |
| nano [file] | Opens the file using the nano editor |
| vim [file] | Opens the file using the vim editor |
| clear |  Clears the screen |
| reset |  Resets the terminal display |


## KOMBINIMI I KOMANDAVE

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| [komanda-a]; [komanda-b] | Ekzekuto komandën A dhe më pas B, pavarësisht nëse komanda A ekzekutohet me sukses apo jo |
| [komanda-a] && [komanda-b] | Ekzekuto komandën B në qoftë se komanda A u ekzekutua me sukses |
| [komanda-a] \|\| [komanda-b] | Ekzekuto komandën B në qoftë se komanda A dështoi |
| [komanda-a] & | Ekzekuto komandën A në background |


## NDËRTHURJA E KOMANDAVE (PIPING)

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| [komanda-a] \| [komanda-b] | Ekzekuto komandën A dhe më pas kaloja rezultatin komandës B. p.sh. `ps auxwww \| grep google |`


## HISTORIKU I KOMANDAVE

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| history n |  Tregon komandat e shtypura në konsolë – shto një numër për të limituar deri në n komandat e fundit |
| Ctrl + r  | Kërkim interaktiv nëpër gjithë komandat e shtypura |
| ![vlerë] |  Ekzekuto komandën e fundit të shtypur në konsolë që fillon me ‘vlerë’ |
| ![vlerë]:p |  Afisho komandën e fundit të shtypur në konsolë që fillon me ‘vlerë’ |
| !! |  Ekzekuto komandën e fundit të shtypur në konsolë |
| !!:p |  Afisho komandën e fundit të shtypur në konsolë |

## MENAXHIMI I SKEDARËVE

|   Komanda  |   Përshkrimi |
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


## MENAXHIMI I DIREKTORIVE

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| mkdir [dir] | Krijo direktori të re |
| mkdir -p [dir]/[dir] |  Krijo direktori të ndërthurura (direktori brenda direktorisë) |
| rmdir [dir] | Fshi direktorinë ( operon vetëm në direktori boshe ) |
| rm -R [dir] | Fshi direktorinë dhe përmbajtjen e saj |
| less [file]|  Output file content delivered in screensize chunks |
| [command] > [file] |  Push output to file, keep in mind it will get overwritten |
| [command] >> [file] | Append output to existing file |
| [command] < [file] |  Tell command to read content from a file |


## KËRKIM

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Kërko për skedarë, e.g. `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Search for all lines that contain the pattern, e.g. `grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | Recursively search in all files in specified directory for all lines that contain the pattern |
| grep -v [search_pattern] [file] | Search for all lines that do NOT contain the pattern |
| grep -i [search_pattern] [file] | Search for all lines that contain the case-insensitive pattern |
| mdfind [search_pattern] | Spotlight search for files (names, content, other metadata), e.g. `mdfind skateboard` |
| mdfind -onlyin [dir] -name [pattern] | Spotlight search for files named like pattern in the given directory |


## NDIHMË

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| [komanda] -h |  Ofron ndihmë |
| [komanda] --help | Ofron ndihmë |
| info [komanda] | Ofron ndihmë |
| man [komanda] |  Tregon manualin e ndihmës/përdorimit për [komandën] |
| whatis [komanda] | Jep përshkrim të shkurtër (me një rresht) të komandës [komandën] |
| apropos [fjala-kyçe] | Kërkon për komanda me fjalën kyçe në përshkrim |
