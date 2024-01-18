# Cursorbewegung

- `h` - nach links
- `j` - nach unten
- `k` - nach oben
- `l` - nach rechts
- `gg` - zur ersten Zeile
- `G` - zur letzten Zeile
- `0` - zum Anfang der Zeile
- `$` - zum Ende der Zeile
- `e` - springt zum Ende eines Worts
- `b` - springt zum Anfang eines Worts
- `ge` - springt rückwärts zum Ende eines Worts
- `w` - springt vorwärts zum Anfang eines Worts
- `str + b` - bewegt den Bildschirm um eine Seite nach oben (Cursor zur letzten Zeile)
- `str + f` - bewegt den Bildschirm um eine Seite nach unten (Cursor zur ersten Zeile)

# Einfügemodus

- `i` - fügt vor dem Cursor ein
- `a` - fügt (anhängt) nach dem Cursor ein
- `o` - fügt eine neue Zeile unter der aktuellen Zeile ein
- `O` - fügt eine neue Zeile über der aktuellen Zeile ein
- `s` - löscht ein Zeichen und ersetzt den Text
- `S` - löscht eine Zeile und ersetzt den Text (entspricht cc)
- `ea` - fügt am Ende des Worts ein

# Markieren von Text

- `v` - startet den visuellen Modus, markiert Zeilen und führt dann einen Befehl aus
	- `y` - kopiert den markierten Text
	- `aw` - markiert ein Wort
	- `d` - löscht den markierten Text
	- `~` - wechselt die Groß- und Kleinschreibung
- `V` - startet den zeilenweisen visuellen Modus
- `str + c` - verlässt den visuellen Modus

# Ausschneiden und Einfügen

- `yy` - kopiert eine Zeile
- `dd` - löscht eine Zeile
- `dw` - löscht (schneidet) die Zeichen des Worts von der Cursorposition bis zum Anfang des nächsten Worts
- `p` - fügt die Zwischenablage nach dem Cursor ein
- `P` - fügt die Zwischenablage vor dem Cursor ein
- `dw` - löscht (schneidet) die Zeichen des Worts von der Cursorposition bis zum Anfang des nächsten Worts
- `di(Zeichen)` - löscht den Inhalt zwischen den angegebenen Zeichen -> `di"` löscht alles zwischen zwei `"`
- `:2,5d` - löscht die Zeilen 2 bis 5

# Beenden

- `:w`
- `:w !sudo tee %` - schreibt die aktuelle Datei mit sudo-Rechten
- `:wq`, `:x`, `ZZ` - schreibt (speichert) und beendet
- `:w!`, `ZQ` - beendet und verwirft nicht gespeicherte Änderungen

# Arbeiten mit mehreren Dateien

- `:tab ba` - legt zwei Dateien als Tabs nebeneinander
	- `gt` - zum nächsten Tab wechseln
	- `gT` - zum vorherigen Tab wechseln

`vim -Od test1 test2` == `vimdiff test1 test2`

