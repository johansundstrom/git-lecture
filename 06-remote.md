# 6. Remote repositories

---

## Mål

* Hämta/lämna från/till central repo
* Kopplingsnamnet - origin

---

## Centralt repo kan vara...

* GitHub (HTTP)
* GIT (Git)
* Delat filutrymme (Local) 
* Terminal (SSH)

---

## Kontrollera användaruppgifter

1. `git config user.name` Visar aktuellt användarnamn för inloggning remote
2. `git config user.email` Visar aktuellt epost för inloggning remote
3. `git config user.name "olleolle"` Ändrar aktuellt användarnamn för inloggning remote
4. `git config user.email "olle@olle.se` Visar aktuellt epost för inloggning remote
5. `git config --list` Visar aktuella inställningar

---

## Anslutning till remote repo

6. `git remote` Notera att inga anslutningar finns
7. `git remote add origin http://github.com/johansundstrom/gitlab.git` 
8. Notera att det går att ansluta till remote repo och hämta data utan giltigt användarnamn och lösenord
9. Gör en förändring i en fil lokalt, Stage'a och Commit'a i Master
10. `git push origin master` Notera att GitHub frågar efter giltigt användarnamn och lösenord
11. Om du fått giltigt användarnamn och lösenord, ställ in dessa enligt p.1-2
12. `git remote` Notera att ```origin``` listas
13. `git remote -v` Lista verbose. Notera (fetch) och (push) adresser
14. `git remote rm origin` Raderar befintliga anslutningar

---

## Hämta filer från centralt repo, skapar lokal mapp samt .git 

15. Med terminalen, gå till lämplig plats i filsystemet `cd <mapp>`
16. _Git clone_ gör följande tre kommandon

* Git init
* Git remote add origin <url>
* Git pull origin master
  
---

## Git Clone

17.  Markera en lämplig plats i filsystemet dit det externa innehållet skall skapas
18.  `git clone http://github.com/johansundstrom/gitlab.git` Skapa lokal mapp och klonar allt
19.  Notera att mapp skapats med `ls`
20.  Gå in i mappen `cd gitlab`
21.  `ls` Notera att det bör finnas ett innehåll
22.  `ls -a` Notera att `.git` mappen finns och är dold
 
---

## Publicera lokala förändringar på ett anslutningsnamn

23. Öppna och redigera fil i mappen gitlab - spara
24. stage'a och commit'a förändringarna
25. `git push http://github.com/johansundstrom/gitlab.git` alternativt `git push origin master`

---

## Git fetch - Hämtar men uppdaterar inte arbetsfiler i HEAD

26. `git fetch http://github.com/johansundstrom/gitlab.git`
27. `git fetch origin` är ett enklare alternativ till ovanstående, kräver etablerad origin

Tips: uppdatera lokal repo innan lokalt arbete inleds. `git fetch` nedladdar filer från central repo, det integrerar inte de lokala arbetsfilerna. Fetch är inte destruktivt.

---

## Git push - Hämtar och uppdaterar arbetsfiler i HEAD

Git clone gör följande två kommandon

* Git fetch
* Git merge origin master
  
28.  `git pull origin master`

* Eftersom `git pull` försöker att göra merge på centrala förändringar med de lokala så är `merge confict` vanligt. 
* Rekommendationen är därför att bara använda `git pull` på ren arbetskopia (lokal repo).
* Ta för vana att alltid uppdatera lokal repo innan lokalt arbete på remote repo inleds

---

Hämtar förändringar från origin och uppdaterar arbetsfiler i HEAD

29.  ```git fetch <url>``` Hämta förändringar från origin
30.  ```git remote``` Lista anslutningar (```origin``` är standard kortnamn på anslutning)
31.  ```git remote -v``` Lista anslutningar verbose

---

(C) Johan Sundström
