# 5. Samarbeten - Branch/Merge

---

## Samarbeten 

* Devisen: *main branch is always deliverable*
* Utveckling testas och verifieras i `branches`
* Vid acceptans sker `merge`

![branch/merge](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)

---

## Aktuell branch

1. Vilken är aktuell branch? 
2. ```git branch``` returnerar antingen `master` eller `main`

---

## Skapa ny branch

2. Skapa ny branch med namnet *develop* ```git branch develop```
3. ```git branch``` Notera grenarna

---

## Byt namn på branch

4. ```git branch --move new_feature``` Flyttar eller döper om aktuell branch till `new_feature`
5.  ```git branch``` Notera aktuell gren

---

## Radera branch

6. ```git branch --delete new_feature``` Raderar branch new_feature

---

## Arbeta på ny branch

7. ```git branch develop``` Skapa på nytt
8. ```git branch``` Notera aktuell gren
9. ```git checkout develop``` Byter till bransch `develop`
10. ```git branch``` Aktuell gren är `develop`

---

## Utveckla i en branch

11. ```touch start.html``` Skapa fil
12. ```ls``` Notera att filen skapades
13. Stage'a och Committ'a nya filen
14. ```git status``` Kontrollera att allt är klart
15. Notera att `start.html` i branch `develop` existerar

---

## Filsystemet vid branchbyte

16. ```git branch``` Aktuell gren är `develop`
17.  Öppna aktuell mapp i Finder eller Filutforskaren
18.  Filen `start.html` finns filsystemet
19.  ```git checkout master``` Byt till `master branch`
20.  Betrakta aktuell mapp i Finder eller Filutforskaren
21.  Filen `start.html` finns INTE filsystemet
22.  ```git checkout master``` Byt till `master branch`

---

## Merge

23. ```git branch``` Notera aktuell bransch
24. ```git checkout master``` Byt till master bransch
25. ```ls``` Notera att `start.html` INTE finns i `master`
26. ```git merge new_feature``` Slår samman 
27. ```ls``` Notera att `start.html` FINNS i `master`

---

## Uppstädning

28. ```git branch -d develop``` Raderar `develop` bransch

--- 

## Use cases

---

## Use Case 1

Skapa en bransch-struktur som passar tre personer som på varsit håll kan utveckla utan att störa vandra. De tre delarna är faster-login, log-bugfix och social-feature i utvecklingsprojektet. Master ska alltid vara _deployable_ och samtliga utvecklare ska ha tillgång en samlad gren.

---

## Use Case 2

Skapa en passande bransch-struktur för en applikation som ständigt utvecklas och skapar major och minor versioner. Master ska alltid vara _deployable_

---

## Use Case 3

Hur skulle en struktur kunna se ut för ett pågående utvecklingsarbete som passar fyra utvecklingsteam (planning, order, lager och fakturering) i en organisation. Planningteamet styr och sammanställer projektet från de tre övriga grupperna. Varje teamledare ansvarar för sitt team på fem person och varje person kan se sidledes och ett steg upp.

---

(C) Johan Sundström