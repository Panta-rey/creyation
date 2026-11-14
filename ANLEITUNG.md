# Neues Projekt auf die Website bringen

1. Im Ordner `projekte` einen neuen Ordner anlegen. Name: klein, ohne Leerzeichen und Umlaute, z. B. `motu-tane-couchtisch`. Der Name wird zur Adresse: creyation.ch/projekte/motu-tane-couchtisch/
2. Die Datei `projekte/_vorlage/index.md` in den neuen Ordner kopieren und ausfüllen. Die Datei muss `index.md` heissen.
3. Die Bilder in denselben Ordner legen. Sie erscheinen in der Reihenfolge ihrer Namen, am einfachsten `01.jpg`, `02.jpg`, `03.jpg` … Das erste Bild ist das Titelbild (oder `titelbild:` in der Datei angeben).
4. Hochladen (auf github.com: im Ordner «Add file» → «Upload files»). Nach ein bis zwei Minuten ist das Projekt online, in der Übersicht, im Filter und mit eigener Seite.

Bilder: am besten JPG, lange Seite etwa 1800–2400 Pixel, nicht mehr als rund 1 MB pro Bild. Handyfotos vorher verkleinern (z. B. am PC «Bilder» → «Grösse ändern»).

Formate: Quer- und Hochformat dürfen gemischt werden. Auf der Projektseite wird kein Bild beschnitten. In der Übersicht und auf der Startseite werden die Bilder auf ein einheitliches Querformat zugeschnitten; ist das erste Bild hochkant, in `index.md` mit `vorschaubild: 02.jpg` ein Querformat-Bild wählen oder mit `ausschnitt: "50% 25%"` den sichtbaren Teil verschieben (erste Zahl links-rechts, zweite oben-unten).

Bereiche für `kategorie`: Raumgestaltung, Inszenierung & Events, Möbel & Objekte, 3D-Druck & Engineering, Camperausbau (mehrere möglich, in eckigen Klammern mit Anführungszeichen).
Das Jahr immer als Zahl ohne Anführungszeichen schreiben, z. B. `jahr: 2024`. Ist das Jahr unbekannt, die Zeile `jahr:` ganz weglassen; das Projekt erscheint dann am Schluss der Übersicht.
Ein Projekt ausblenden, ohne es zu löschen: in `index.md` oben die Zeile `published: false` einfügen. Zum Einblenden die Zeile wieder löschen.
Ordner, deren Name mit `_` beginnt (wie `_vorlage`), erscheinen nicht auf der Website.

# Neues Produkt auf die Website bringen

Genau wie bei den Projekten: ein Ordner pro Produkt.

1. Im Ordner `produkte` einen neuen Ordner anlegen. Name: klein, ohne Leerzeichen und Umlaute, z. B. `kinderzimmer-regal`. Der Name wird zur Adresse: creyation.ch/produkte/kinderzimmer-regal/
2. Die Datei `produkte/_vorlage/index.md` in den neuen Ordner kopieren und ausfüllen (Name, Linie, Kurztext; Masse, Reihenfolge und Farben sind freiwillig).
3. Die Bilder in denselben Ordner legen, am einfachsten `01.jpg`, `02.jpg` … Das erste Bild ist das Hauptbild, die übrigen erscheinen als kleine Vorschau in der Übersicht und gross auf der Produktseite. Kein Bild wird beschnitten.
4. Hochladen. Das Produkt erscheint in der Übersicht in seiner Linie und bekommt eine eigene Seite.

Linien: Home, Haustiere, Werkstatt. Farbwahl: siehe Beispiel in der Vorlage oder im Ordner `produkte/vitruvius`.

# Texte und Bilder selbst ändern

Alle Texte der festen Seiten stehen in einfachen Textdateien im Ordner `_data`. Öffnen mit dem Editor (Notepad), ändern, speichern, hochladen.

| Was | Datei |
|---|---|
| Startseite: alle Texte und Bilder | `_data/startseite.yml` |
| Kundenliste auf der Startseite | `_data/kunden.yml` |
| Seite «Über mich» | `_data/ueber_mich.yml` |
| Kontaktbereich (Titel, Text, Adressen) | `_data/kontakt.yml` |
| Katzensofa: Texte, Stoffe, Holztöne | `_data/katzensofa.yml` |

Regeln (stehen auch oben in jeder Datei):

- Nur den Text zwischen den Anführungszeichen `"..."` ändern. Die Wörter vor dem Doppelpunkt und die Einrückung am Zeilenanfang nicht ändern.
- Im Text keine geraden Anführungszeichen `"` schreiben, sondern « ».
- Bilder der Startseite liegen in `assets/bilder/start/`. Neues Bild dort ablegen und in der Datei den Namen eintragen, z. B. `bild: start/mein-bild.jpg`.
- Bleibt die Seite nach dem Hochladen unverändert, hat sich meist ein Tippfehler in eine dieser Dateien eingeschlichen (fehlendes Anführungszeichen, verschobene Einrückung). Auf github.com unter «Actions» steht dann ein roter Lauf mit der Zeilennummer.

Die sechs Projekte auf der Startseite werden nicht hier gewählt, sondern in den Projekten mit `startseite: 1` bis `6`.

# Katzensofa: Kombinationen von Stoff und Holz

Jede Kombination ist ein Foto im Ordner `assets/bilder/casadelpaw/` mit dem Namen `stoff-holz.jpg`, z. B. `haifa-cognac.jpg`. Foto hineinlegen = Kombination ist wählbar; Foto löschen = nicht mehr wählbar. Eintragen muss man dafür nichts.

Neuer Stoff: in `_data/katzensofa.yml` unter `stoffe:` eine Zeile ergänzen (Kurzname `id`, angezeigter Name, Farbton) und mindestens ein Foto `kurzname-natur.jpg` ablegen. Bilder für «Happy Clients»: alle Dateien im selben Ordner, deren Name mit `happy-` beginnt.
