# 3. Filhantering i Bash

---

## Agenda

* Skapa/lista
* Rättigheter
* Chmod

---

## Skapa/lista

1. Öppna `git bash` terminalen
2. Med `cd <mapp>` och `mkdir <ny mapp>` gå till lämplig plats i filsystemet (Mina dokument/proj)
3. Sänd `ls` (list) konstatera att det är tomt
4. Sänd `touch index.html` Skapa index.html
5. Sänd `ls`. Skapad?

---

## Rättigheter

6. Sänd `ls -l` (listar rättigheter)
Bokstäverna rwx står för Read/Write/Execute rättighet. Dessa visas tre gånger, först för `Owner`, därefter `Group` och sist `Others` (world). RWX benämns ibland 7 (1+2+4). Första biten kan vara - (fil) eller d (katalog)
7. Sänd `ls -full` (lista allt)
8. Sänd `ls -a` (lista mappar som börjar med dot)
9. Sänd `ls -a -full` (lista utökat och mappar som börjar med dot)

---

## Chmod (Change mode)

10. Besvara: När skapades filen?
11. Vad har filen för filrättigheter?
12. Läs om [chmod](https://ss64.com/bash/chmod.htm)

---

## Kontrollera Git

13. `git status` visar om mappen är ett repo
14. Sänd `ls -a`
15. Besvara: Vad har filen `index.html` för status (untracked | staged | committed ) och färg?

---

## Redigera fil

16. Redigera filen `index.html` med t.ex. `<html>...</html>` och spara (Mac: `open -a textedit index.html` | Windows: `notepad index.html` | Linux: `nano index.html`)
17. Spara
ß
--- 

(C) Johan Sundström