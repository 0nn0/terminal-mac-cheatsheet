# Terminal Cheatsheet für Mac (Grundlagen)

_Zur besseren Lesbarkeit werden die Buchstaben groß geschrieben._  _Capslock sollte ausgeschaltet sein._

------------

### ABKÜRZUNGEN

| Schlüssel/Befehl | Beschreibung |
| ----------- | ----------- |
| ctrl + A | Zum Anfang der Zeile, in der Sie gerade tippen, gehen.  Dies funktioniert auch für die meisten Texteingabefelder im gesamten System.  Netbeans bildet hier eine Ausnahme.
| ctrl + E | Gehe zum Ende der Zeile, in der du gerade schreibst.  Dies funktioniert auch für die meisten Texteingabefelder im gesamten System.  Netbeans bildet eine Ausnahme.
| ctrl + L | Bildschirm löschen |
| Cmd + K | Bildschirm leeren |
| ctrl + U | Alles rückwärts bis zum Zeilenanfang ausschneiden |
| ctrl + K | Alles vorwärts bis zum Ende der Zeile ausschneiden |
| ctrl + W | Ein Wort rückwärts ausschneiden mit Leerzeichen als Trennzeichen |
| ctrl + Y | Einfügen, was mit dem letzten Ausschneidebefehl ausgeschnitten wurde |
| ctrl + H | Wie die Rücktaste |
| ctrl + C | Beendet das Programm, das Sie gerade ausführen.  Löscht auch alles in der aktuellen Zeile.
| ctrl + D | Beendet die aktuelle Shell, wenn kein Prozess läuft, oder sendet EOF an einen laufenden Prozess |
| ctrl + Z | Versetzt den laufenden Prozess in einen angehaltenen Hintergrundprozess. fg stellt ihn wieder her.
| ctrl + _ | Macht den letzten Befehl rückgängig. (Unterstrich. Es ist also eigentlich ctrl + Shift + Minus) |
| ctrl + T | Vertauscht die letzten beiden Zeichen vor dem Cursor |
| ctrl + F | Bewegt den Cursor um ein Zeichen nach vorne |
| ctrl + B | Bewegt den Cursor um ein Zeichen zurück |
| Option + → | Cursor ein Wort vorwärts bewegen |
| Option + ← | Cursor ein Wort rückwärts bewegen |
| Esc + T | Vertauscht die letzten beiden Wörter vor dem Cursor |
| Esc + Backspace | Ein Wort rückwärts ausschneiden, ohne Buchstaben als Trennzeichen zu verwenden |
| Tabulator | Automatisches Vervollständigen von Datei- und Ordnernamen |

### WICHTIGSTE BEFEHLE

| Schlüssel/Befehl | Beschreibung |
| ----------- | ----------- |
| cd [Ordner] | Verzeichnis wechseln z.B. `cd Dokumente` |
| cd | Heimatverzeichnis |
| cd ~ | Hauptverzeichnis |
| cd / | Wurzel des Laufwerks |
| cd - | Vorheriges Verzeichnis |
| ls | Kurze Auflistung |
| ls -l | Lange Auflistung |
| ls -a | Auflistung inkl. versteckter Dateien |
| ls -lh| Lange Auflistung mit menschenlesbaren Dateigrößen |
| ls -R | Gesamter Inhalt eines Ordners rekursiv |
| sudo [Befehl] | Befehl mit den Sicherheitsrechten des Superusers (Super User DO) ausführen |
| open [file] | Öffnet eine Datei (als ob Sie auf sie doppelklicken würden) |
| top | Zeigt aktive Prozesse an. Drücken Sie q zum Beenden |
| nano [datei] | Öffnet die Datei mit dem nano-Editor |
| vim [Datei] | Öffnet die Datei mit dem vim-Editor |
| clear | Löscht den Bildschirm |
| reset | Setzt die Terminalanzeige zurück |

### BEFEHLSKETTEN

| Key/Command | Description |
| ----------- | ----------- |
| [command-a]; [command-b] | Führen Sie den Befehl A und dann B aus, unabhängig vom Erfolg von A |
| [command-a] && [command-b] | Befehl B ausführen, wenn A erfolgreich war |
| [command-a] \|\| [command-b] | Befehl B ausführen, wenn A fehlgeschlagen ist |
| [command-a] & | Befehl A im Hintergrund ausführen |


### PIPING-BEFEHLE

| Key/Command | Description |
| ----------- | ----------- |
| [command-a] \| [command-b] | Führen Sie Befehl A aus und übergeben Sie das Ergebnis an Befehl B, z. B. ps auxwww \| grep google |


### BEFEHLSVERLAUF

| Schlüssel/Befehl | Beschreibung |
| ----------- | ----------- |
| Historie n | Zeigt die eingegebenen Befehle an - fügen Sie eine Zahl hinzu, um die letzten n Einträge zu begrenzen |
| ctrl + r | Interaktives Durchsuchen zuvor eingegebener Befehle |
| ![Wert] | Führt den zuletzt getippten Befehl aus, der mit 'Wert' beginnt |
| ![Wert]:p | Druckt den zuletzt eingegebenen Befehl, der mit 'Wert' beginnt, auf der Konsole aus |
| !! | Ausführen des zuletzt getippten Befehls |
| !!:p | Ausgabe des zuletzt eingegebenen Befehls auf der Konsole |

### DATEIVERWALTUNG

| Schlüssel/Befehl | Beschreibung |
| ----------- | ----------- |
| touch [Datei] | Erstellen einer neuen Datei |
| pwd | Vollständiger Pfad zum Arbeitsverzeichnis |
| . | Aktueller Ordner, z.B. `ls .` |
| .. | Übergeordnetes/umschließendes Verzeichnis, z. B. `ls ..` |
| ls -l .. | Lange Auflistung des übergeordneten Verzeichnisses |
| cd ../../ | 2 Ebenen nach oben gehen |
| cat | Konkatenieren auf dem Bildschirm |
| rm [Datei] | Entfernen einer Datei, z.B. "rm data.tmp" |
| rm -i [Datei] | Entfernen mit Bestätigung |
| rm -r [dir] | Ein Verzeichnis und dessen Inhalt entfernen |
| rm -f [file] | Erzwingen des Entfernens ohne Bestätigung |
| cp [datei] [newfile] | Datei in Datei kopieren |
| cp [datei] [dir] | Kopieren einer Datei in ein Verzeichnis |
| mv [datei] [neuer dateiname] | Verschieben/Umbenennen, z.B. `mv datei1.ad /tmp` |
| pbcopy < [file] | Kopiert den Inhalt einer Datei in die Zwischenablage |
| pbpaste | Einfügen des Inhalts der Zwischenablage |
| pbpaste > [Datei] | Inhalt der Zwischenablage in Datei einfügen, z.B. "pbpaste > paste-test.txt" |

### VERZEICHNISVERWALTUNG

| Schlüssel/Befehl | Beschreibung |
| ----------- | ----------- |
| mkdir [dir] | Neues Verzeichnis erstellen |
| mkdir -p [dir]/[dir] | Verschachtelte Verzeichnisse erstellen |
| rmdir [dir] | Verzeichnis entfernen (funktioniert nur bei leeren Verzeichnissen) |
| rm -R [dir] | Verzeichnis und Inhalt entfernen |
| less [file]| Dateiinhalt in Bildschirmgröße ausgeben |
| [befehl] > [datei] | Ausgabe in Datei verschieben, beachten Sie, dass sie überschrieben wird |
| [befehl] >> [datei] | Ausgabe an vorhandene Datei anhängen |
| [befehl] < [datei] | Dem Befehl sagen, dass er den Inhalt aus einer Datei lesen soll |

### SUCHE

| Schlüssel/Befehl | Beschreibung |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Suche nach Dateien, z.B. `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Suche nach allen Zeilen, die das Muster enthalten, z.B. `grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | Rekursive Suche in allen Dateien im angegebenen Verzeichnis nach allen Zeilen, die das Muster enthalten |
| grep -v [search_pattern] [file] | Suche nach allen Zeilen, die das Muster NICHT enthalten |
| grep -i [search_pattern] [file] | Suche nach allen Zeilen, die das Muster ohne Berücksichtigung der Groß-/Kleinschreibung enthalten |
| mdfind [search_pattern] | Spotlight-Suche nach Dateien (Namen, Inhalt, andere Metadaten), z.B. `mdfind skateboard` |
| mdfind -onlyin [dir] -name [muster] | Spotlight-Suche nach Dateien mit dem Namen des Musters im angegebenen Verzeichnis |

### HILFE

| Schlüssel/Befehl | Beschreibung |
| ----------- | ----------- |
| [Befehl] -h | Bietet Hilfe an |
| [Befehl] --help | Bietet Hilfe an |
| info [Befehl] | Bietet Hilfe an |
| man [Befehl] | Zeigt das Hilfehandbuch für [Befehl] an |
| whatis [Befehl] | Gibt eine einzeilige Beschreibung von [Befehl] an |
| apropos [search-pattern] | Sucht nach Befehl mit Schlüsselwörtern in der Beschreibung |