# 5. Samarbeten - Branch/Merge

---

## Samarbeten 

* Devisen: *main branch is always deliverable*
* Utveckling testas och verifieras i `branches`
* Vid acceptans sker `merge`

![branch/merge](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)

---

## Aktuell branch

1. Vilken är aktuell branch? ```git branch``` returnerar antingen `master` eller `main`

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

5. ```git branch develop``` Skapa på nytt
6. ```git branch``` Notera aktuell gren
7. ```git checkout develop``` Byter till branch `develop`
8. ```git branch``` Aktuell gren är `develop`

---

## 1. Utveckla i en branch

9. ```touch start.html``` Skapa fil
10. ```ls``` Notera att filen skapades
11. Stage'a och Committ'a nya filen
12. ```git status``` Kontrollera att allt är klart
13. Notera att filen i branch `develop` existerar

## 2. Utveckla i en branch

14. ```git checkout master``` Byt till `master branch`
17. ```ls``` Filen `start.html` ska inte finnas i `master branch`
18. Bevaka mappen i Finder eller Filutforskaren vid bytet
19. Notera att endast filer från Master existerar
20. ```git checkout new_feature``` Byt till New_Feature
21. Sänd ```ls```
22. Notera att filer från Master och New_Feature existerar
23. ```git log --oneline --decorate --graph --all -5``` Lista de 5 senaste händelserna

---

## Merge

23. ```git branch``` Notera aktuell branch
24. ```git checkout master``` Byt till master branch
25. ```ls``` Notera att ```content.txt``` INTE finns i ```Master```
26. ```git merge new_feature``` Slår samman ```new_feature```med aktuell branch (```master```)
27. ```ls``` Notera att ```content.txt``` FINNS i ```Master```

---

## Uppstädning

28. ```git branch -d new_feature``` Raderar develop branch

--- 

## Use cases

29. Besvara: Skapa en branch-struktur som passar tre personer som på varsit håll kan utveckla utan att störa vandra. De tre delarna är faster-login, log-bugfix och social-feature i utvecklingsprojektet. Master ska alltid vara _deployable_ och samtliga utvecklare ska ha tillgång en samlad gren.

30. Besvara: Skapa en passande branch-struktur för en applikation som ständigt utvecklas och skapar major och minor versioner. Master ska alltid vara _deployable_

31. Besvara: Hur skulle en struktur kunna se ut för ett pågående utvecklingsarbete som passar fyra utvecklingsteam (planning, order, lager och fakturering) i en organisation. Planningteamet styr och sammanställer projektet från de tre övriga grupperna. Varje teamledare ansvarar för sitt team på fem person och varje person kan se sidledes och ett steg upp.

---

(C) Johan Sundström