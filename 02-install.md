# 2. Installera Git

---

## Mål

* Instruktioner för att installera och konfigurera Git

---

## 1. Installera

<img src="https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png" width="10%" height="10%" />


1. [https://git-scm.com](https://git-scm.com)
2. Installera `Git` för ditt operativsystem
3. Acceptera alla förvalda inställningar

---

## 2. Skapa konto på Github

1. [https://github.com](https://github.com)
2. Kontot behövs för git

---

## 3. Konfigurera Git

1. Öppna bash terminal 
2. `mkdir <mapp>` och `cd <mapp>` - Skapar och flyttar till nya mappen i lokala filsystemet 
3. `git init` - Skapar lokal repository med systemfiler i dolda undermappen `.git`
4. `git config --global user.name "johansundstrom"` - Tillägget `--global` ger åtkomst i alla projektmappar
5. `git config --global user.email "johan.sundstrom@mdh.se"`

---

## 4. Konfigurera Git

5. `git config user.name` - Visar användarnamn
6. `git config user.email` - Visar epostadress
7. `git config --list` - Listar inställningar
8. `git config --global user.name "ninja-johan"` - Ändrar username
9. `git config --global color.ui auto` - Färg UI

---

## 5. Hjälp

1. `git <verb> --help`
2. `git help <verb>`

--- 

(C) Johan Sundström