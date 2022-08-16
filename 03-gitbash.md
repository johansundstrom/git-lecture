# 3. Filhantering med Bash

---

## Mål

* Förkunskaper för terminalläget
* Intro till vanliga bash-kommandon (Linuxterminal)

---

## Agenda

* Skapa/lista
* Rättigheter
* Chmod

---

## Skapa- lista mappar och filer

1. Öppna `git bash` terminalen
2. Med `cd <mapp>` och `mkdir <ny mapp>` gå till lämplig plats i filsystemet (Mina dokument/proj)
3. Sänd `ls` (list) konstatera att det är tomt
4. Sänd `touch index.html` Skapa index.html
5. Sänd `ls`. Skapad?

---

## Rättigheter

6. Sänd `ls -l` - Listar rättigheter
Bokstäverna rwx står för Read/Write/Execute rättighet. Dessa visas tre gånger, först för `Owner`, därefter `Group` och sist `Others` (world). RWX benämns ibland 7 (1+2+4). Första biten kan vara `-` fil eller `d` directory (mapp)
7. Sänd `ls -full` - Lista allt
8. Sänd `ls -a` - Listar även dolda mappar som börjar med dot
9. Sänd `ls -a -full` listar utökat och dolda mappar
10. Besvara: När skapades filen?
11. Vad har filen för filrättigheter?

---

## Chmod (Change mode)

* Chmod ändrar filrättigheter
* Syntax: 
 
```chmod u=rw, g=r, o=r index.html``` 


12.   Läs mer om [chmod](https://ss64.com/bash/chmod.htm)

---

## Kontrollera Git

13.  `git status` visar status och om mappen är ett repo
14.  Sänd `ls -a`
15.  Besvara: Vad har filen `index.html` för status (untracked | staged | committed ) och färg?

---

## Redigera fil

16. Redigera filen `index.html` med t.ex. `<html>...</html>` och spara (Mac: `nano index.html` | Windows: `notepad index.html` | Linux: `nano index.html`)
17. Spara

--- 

(C) Johan Sundström