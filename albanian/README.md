
# Përmbledhje e komandave të Terminalit për Mac (Bazat)

------------

_Shkronjat janë në versionin kapital për t'u lexuar më lehtë._  _Butoni Capslock duhet të jetë i fikur._


## SHKURTIME

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| Ctrl + A   | Shko në fillim të rreshtit që je duke shkruar. Kjo funksionon edhe për shumicën e inputeve text në mbarë sistemin. Netbeans përbën përjashtim |
| Ctrl + E   | Shko në fund të rreshtit që je duke shkruar. Kjo funksionon edhe për shumicën e inputeve text në mbarë sistemin. Netbeans përbën përjashtim |
| Ctrl + L   | Pastron/Fshin ekranin |
| Cmd + K    | Pastron/Fshin ekranin |
| Ctrl + U   | Cut everything backwards to beginning of line |
| Ctrl + K   | Cut everything forward to end of line |
| Ctrl + W   | Cut one word backwards using white space as delimiter |
| Ctrl + Y   | Ngjit çfarëdo që është prerë në përdorimin e fundit të komandës prij/cut. |
| Ctrl + H   | E njëjtë me komandën backspace |
| Ctrl + C   | Kill whatever you are running.  Also clears everything on current line |
| Ctrl + D   | Exit the current shell when no process is running, or send EOF to a the running process |
| Ctrl + Z   | Puts whatever you are running into a suspended background process. fg restores it |
| Ctrl + _   | Undo the last command. (Underscore.  So it's actually Ctrl + Shift + minus) |
| Ctrl + T   | Swap the last two characters before the cursor |
| Ctrl + F   | Zhvendos kursorin një karakter përpara. |
| Ctrl + B   | Zhvendos kursorin një karakter pas. |
| Option + →  | Zhvendos kursorin një fjalë përpara. |
| Option + ←  | Zhvendos kursorin një fjalë pas. |
| Esc + T  | Shkëmbe vendndodhjet e dy fjalëve të fundit para kursorit |
| Esc + Backspace | Cut one word backwards using none alphabetic characters as delimiters |
| Tab  | Kompleto automatikisht emrat e skedarëve dhe direktorive |


## KOMANDAT THEMELORE

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| cd [direktoria] | Ndrysho direktorinë e.g. `cd Documents` |
| cd |  direktoria bazë (Home) |
| cd ~ |  direktoria bazë (Home) |
| cd /  | Rrënja e diskut |
| cd -  | Direktoria e mëparshme |
| ls | Listim i shkurtër (në rresht) |
| ls -l | Listim i gjatë (në kolonë) |
| ls -a | Listimi përfshin skedarët e fshehur |
| ls -lh| Listim i gjatë me madhësitë e skedarëve në format të lexueshëm për njeriun |
| ls -R | Liston të gjithë përmbajtjen e direktorisë rekursivisht |
| sudo [komanda] | Ekzekuto komandën me privilegjet e superpërdoruesit (Super User DO) |
| open [skedari] | Hap një skedar ( njëlloj sikur do hapej duke klikuar ) |
| top | Afishon proçeset aktive. Shtyp q për të dalë |
| nano [skedari] | Hap skedarin duke përdorur editorin nano |
| vim [skedari] | Hap skedarin duke përdorur editorin vim |
| clear |  Pastron/fshin ekranin |
| reset |  Rivendos/reseton ekranin e terminalit |


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
| find [dir] -name [shprehja-] | Kërko për skedarë, e.g. `find /Users -name "file.txt"` |
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
