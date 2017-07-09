# Ściągawka skrótów klawiszowych w konsoli Mac (Podstawy)


------------

_Skróty są pisane wielkimi literami tylko ze wględu na czytelność._  _Capslock powinien pozostać niewciśnięty._
## SKRÓTY KLAWISZOWE

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| Ctrl + A   | Idź do początku obecnej linii.  Działa także dla większości pól tekstowych w systemie. Środowisko Netbeans jest wyjątkiem |
| Ctrl + E   | Idź do końca obecnej linii.  Działa także dla większości pól tekstowych w systemie. Środowisko Netbeans jest wyjątkiem |
| Ctrl + Q   | Czyści całą obecną linię|
| Ctrl + L   | Czyści ekran|
| ⌘Cmd + K |Czyści ekran |
| Ctrl + U   | Wytnij wszystko przed początkiem linii |
| Ctrl + K   | Wytnij wszystko za końcem linii |
| Ctrl + W   | Wytnij poprzednie słowo oddzielone spacją |
| Ctrl + Y   | Wstaw to co ostatnio zostało wycięte |
| Ctrl + H   | Działa jak klawisz backspace |
| Ctrl + C   | Przerwij obecnie trwający proces |
| Ctrl + D   | Wychodzi z powłoki gdy nie trwa zaden proces, w przeciwnym wypadku wysyła sygnał EOF do trwającego procesu. |
| Ctrl + Z   | Przenosi obecnie działający proces do zamrozonego procesu w tle. fg zeby go wznowić. |
| Ctrl + _   | Cofnij ostatnie polecenie. (Podkreślnik.  Właściwie Ctrl + Shift + minus) |
| Ctrl + T   | Zamień dwa ostatnie znaki za kursorem |
| Ctrl + F   | Przesuń kursor o jeden znak do przodu |
| Ctrl + B   | Przesuń kursor o jeden znak do tyłu |
| Esc + F  | Przesuń kursor o jedno słowo do przodu |
| Esc + B  | Przesuń kursor o jedno słowo do tyłu |
| Esc + T  | Zamień dwa ostatnie słowa za kursorem |
| Tab  | Auto-wypełnienie nazw plików i katalogów |

## PODSTAWOWE POLECENIA

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| cd |  Katalog domowy |
| cd [folder] | Zmiana katalogu na przykład `cd documents` |
| cd /  | Katalog źródłowy |
| cd -  | Poprzedni katalog |
| ls | Krótki wykaz zawartości katalogu |
| ls -l | Szczegółowy wykaz zawartości katalogu |
| ls -a | Wykaz zawartości katalogu zawierający ukryte pliki |
| ls -lh| Szczegółowy wykaz zawartości katalogu z czytelnymi rozmiarami plików |
| ls -R | Entire content of folder recursively |
| sudo [polecenie] | Wykonaj polecenie z uprawnieniami superuzytkownika (Super User DO) |
| open [plik] | Otwiera plik ( analogicznie jak przy podwójnym wciśnięciu ) |
| top | Wyświetla aktywne procesy. Wciśnij q zeby wyjść |
| nano [plik] | Otwiera plik w edytorze nano |
| vim [plik] | Otwiera plik w edytorze vim |
| clear |  Czyść ekran |
| reset |  Resetuje ekran konsoli |

## ŁĄCZENIE POLECEŃ

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| [polecenie-a]; [polecenie-b] | Wykonaj polecenie A i potem B, niezaleznie od powodzenia A |
| [polecenie-a] && [polecenie-b] | Wykonaj polecenie B jeśli A się powiedzie |
| [polecenie-a] || [polecenie-b] | Wykonaj polecenie B jeśli A się nie powiedzie |
| [polecenie-a] & | Wykonaj polecenie A w tle |


## PRZEKAZYWANIE POLECEŃ

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| [polecenie-a] \| [polecenie-b] | Wykonaj polecenie A i przekaz wynik do polecenia B na przykład ps auxwww \| grep google |


## HISTORIA POLECEŃ

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| history n |  Wyświetl historię wpisanych poleceń – n ogranicza liczbę wyników do n poleceń |
| Ctrl + r  | Przeszukuj ostatnio wpisane polecenia |
| ![wartość] |  Wykonaj ostatnie polecenie zaczynające się na ‘wartość’ |
| !! |  Wykonaj ostatnio wykonane polecenie |

## ZARZĄDZANIE PLIKAMI

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| touch [plik] |   Tworzy nowy plik |
| pwd | Pełna ściezka do katalogu roboczego |
| . |  Obecny katalog, na przykład `ls .` |
| .. | Nadrzędny katalog, na przykład `ls ..` |
| `ls -l ..` | Szczegółowy wykaz katalogu nadrzędnego katalog |
| `cd ../../` | Przemieść się dwa poziomy katalogów w górę |
| cat | Wyświetl na ekranie |
| rm [plik] |  Usuń plik, na przykład `rm data.tmp` |
| rm -i [plik] | Usuń plik z potwierdzeniem |
| rm -r [kat] | Usuń katalog i jego zawartość |
| rm -f [plik] | Usuń plik bez potwierdzenie |
| cp [plik] [nowy plik] | Skopiuj plik to pliku |
| cp [plik] [kat] | Skopiuj plik to katalogu |
| mv [plik] [nowa nazwa pliku] |  Przenieś/Zmień nazwę pliku, na przykład `mv plik1.ad /tmp` |
| pbcopy < [plik] | Kopiuj zawartość pliku to schowka |
| pbpaste | Wklej zawartość schowka |
| pbpaste > [plik] | Wklej zawartość schowka do pliku, `pbpaste > paste-test.txt` |

## ZARZĄDZANIE KATALOGAMI

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| mkdir [kat] | Tworzy nowy katalog |
| mkdir -p [kat]/[kat] |  Tworzy zagniezdzone katalogi |
| rmdir [kat] | Usuń katalog ( działa tylko na pustych katalogach) |
| rm -R [kat] | Usuń katalog i jego zawartość |
| [polecenie] \| [polecenie] | Pozwala na łączenie kilku poleceń generujących dane, na przykład `cat data.txt | pbcopy` |
| less |  Output content delivered in screensize chunks |
| [polecenie] > [plik] |  Nadpisz plik wynikiem polecenia |
| [polecenie] >> [plik] | Dołącz do istinejącego pliku |
| [polecenie] < [plik] |  Przekaz zawartość pliku do polecenia |

## WYSZUKIWANIE

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| find [kat] -nazwa [wzorzec] | Szukaj plików, na przykład `find /Users -name "plik.txt"` |
| grep [wzorzec] [plik] | Szukaj wszystkich linii zawierających wzorzec, na przykład `grep "Tom" plik.txt` |
| grep -r [wzorzec] [plik] | Rekursywnie szukaj wyszstkich linii zawierających wzorzec |
| grep -v [wzorzec] [plik] | Szukaj wszystkich linii NIE zawierających wzorca |

## POMOC

|  Klawisz/e  |    Opis     |
| ----------- | ----------- |
| [polecenie] -h |  Wyświetla pomoc |
| [polecenie] —help | Wyświetla pomoc |
| info [polecenie] | Wyświetla pomoc |
| man [polecenie] |  Wyświetla instrukcję polecenia |
| whatis [polecenie] | Wyświetla jednolinijkowy opis polecenia |
| apropos [search-pattern] | Szuka poleceń ze słowami kluczowymi w opisie |
