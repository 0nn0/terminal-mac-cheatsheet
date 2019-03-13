
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
| Ctrl + U   | Prij përmbajtjen nga pozicioni aktual i kursorit deri në fillim të rreshtit |
| Ctrl + K   | Prij përmbajtjen nga pozicioni aktual i kursorit deri në fund të rreshtit |
| Ctrl + W   | Prij një fjalë para nga pozicioni aktual i kursorit |
| Ctrl + Y   | Ngjit çfarëdo që është prerë në përdorimin e fundit të komandës prij/cut. |
| Ctrl + H   | E njëjtë me komandën backspace |
| Ctrl + C   | Ndalo çfarëdo që je duke ekzekutuar në konsolë.  Gjithashtu fshin përmbajtjen e rreshtit aktual |
| Ctrl + D   | Dil nga terminali shell kur asnjë proçes nuk është duke punuar, ose dërgo sinjalin EOF proçesit që është duke punuar |
| Ctrl + Z   | Vendos çfarëdo që është duke u ekzekutuar në një proçes të pezulluar në background |
| Ctrl + _   | Kthe përsëri komandën e fundit. (Vijë poshtë.  Pra realisht është Ctrl + Shift + minus) |
| Ctrl + T   | Shkëmbe vendndodhjet e dy karaktereve të fundit para kursorit |
| Ctrl + F   | Zhvendos kursorin një karakter përpara. |
| Ctrl + B   | Zhvendos kursorin një karakter pas. |
| Option + →  | Zhvendos kursorin një fjalë përpara. |
| Option + ←  | Zhvendos kursorin një fjalë pas. |
| Esc + T  | Shkëmbe vendndodhjet e dy fjalëve të fundit para kursorit |
| Esc + Backspace | Prij një fjalë para nga pozicioni aktual i kursorit duke përdorur si ndarës karaktere jo shkronja |
| Tab  | Kompleto automatikisht emrat e skedarëve dhe direktorive |


## KOMANDAT THEMELORE

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| cd [direktoria] | Ndrysho direktorinë p.sh. `cd Documents` |
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
| touch [skedari] | Krijo një skedar të ri |
| pwd | Afisho adresën e plotë e direktorisë aktuale |
| . |  Direktoria aktuale, p.sh. `ls .` |
| .. | Direktoria prind, p.sh. `ls ..` |
| ls -l .. | Listim i gjatë i direktorisë prind |
| cd ../../ | Zhvendosu 2 nivele më lartë |
| cat | Bashkangjit në ekran |
| rm [skedari] |  Fshi një skedar, p.sh. `rm data.tmp` |
| rm -i [skedari] | Fshi duke konfirmuar |
| rm -r [dir] | Fshi një direktori dhe përmbajtjen e saj |
| rm -f [skedari] | Fshi me forcë pa konfirmim |
| cp [skedari] [skedari-i-ri] | Kopjo skedarin në skedarin e ri |
| cp [skedari] [dir] | Kopjo skedarin në direktori |
| mv [skedari] [emri i ri] |  Zhvendos/Riemërto, p.sh. `mv file1.ad /tmp` |
| pbcopy < [skedari] | Kopjo përmbajtjen e skedarit në clipboard |
| pbpaste | Ngjit/Shkruaj përmbajtjen e clipboard |
| pbpaste > [skedari] | Ngjit/Shkruaj përmbajtjen e clipboard në një skedar, `pbpaste > paste-test.txt` |


## MENAXHIMI I DIREKTORIVE

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| mkdir [dir] | Krijo direktori të re |
| mkdir -p [dir]/[dir] |  Krijo direktori të ndërthurura (direktori brenda direktorisë) |
| rmdir [dir] | Fshi direktorinë (operon vetëm në direktori boshe) |
| rm -R [dir] | Fshi direktorinë dhe përmbajtjen e saj |
| less [skedari]|  Afisho përmbajtjen e skedarit në copa të barabarta me madhësinë e ekranit |
| [komanda] > [skedari] |  Vendos outputin në skedar, kij parasysh që përmbajta do të mbishkruhet |
| [komanda] >> [skedari] | Shto outputin në një skedar ekzistues (shtim në fund) |
| [komanda] < [skedari] |  Udhëzo komandën të lexojë përmbajtjen nga skedari |


## KËRKIM

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| find [dir] -name [fjala-kyçe] | Kërko për skedarë, p.sh. `find /Users -name "file.txt"` |
| grep [fjala-kyçe] [skedari] | Kërko për të gjitha rreshtat që përmbajnë fjalën kyçe, p.sh. `grep "Tom" file.txt` |
| grep -r [fjala-kyçe] [dir] | Rekursivisht kërko në të gjithë skedarët në direktorinë e specifikuar për të gjitha rreshtat që përmbajnë fjalën kyçe |
| grep -v [fjala-kyçe] [skedari] | Kërko për të gjitha rreshtat që NUK përmbajnë fjalën kyçe |
| grep -i [fjala-kyçe] [skedari] | Kërko për të gjitha rreshtat që përmbajnë fjalën kyçe ekzakte (Kapitalizimi i shkronjave ka rëndësi) |
| mdfind [fjala-kyçe] | Kërkim i shpejtë për skedarë (emri, përmbajtja, metadata të tjera), p.sh. `mdfind skateboard` |
| mdfind -onlyin [dir] -name [fjala-kyçe] | Kërkim i shpejtë për skedarë të emëruar si paterni në direktorinë e dhënë |


## NDIHMË

|   Komanda  |   Përshkrimi |
| ----------- | ----------- |
| [komanda] -h |  Ofron ndihmë |
| [komanda] --help | Ofron ndihmë |
| info [komanda] | Ofron ndihmë |
| man [komanda] |  Tregon manualin e ndihmës/përdorimit për [komandën] |
| whatis [komanda] | Jep përshkrim të shkurtër (me një rresht) të komandës [komandën] |
| apropos [fjala-kyçe] | Kërkon për komanda me fjalën kyçe në përshkrim |
