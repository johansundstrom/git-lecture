# 4. Versionshantering

---

## Agenda

* Repository/repo (förråd)
* Snapshots

---

## Versionskontroll

* Versionshantering menas att en mapp eller fil's innehåll kan finnas i olika versioner.
* Möjlighet att backa till tidigare version finns.

---

## Tänk Snapshots

---

## Tillståndshantering

<img src="https://camo.githubusercontent.com/68c10cf9817f61108313cf3eb561e96913e0f16783a31e344f1414e11dbe41a1/68747470733a2f2f6769742d73636d2e636f6d2f696d616765732f61626f75742f696e646578314032782e706e67">

---

## Stage fil

1. ```git add index.html```
2. ```git status```
3. Besvara: Vad har filen index.html för status och färg?

---

## Unstage fil

4. ```git reset HEAD index.html``` Fungerar det inte så använd ```git rm --cached index.html```
5. ```git status```

---

## Commit fil

6. ```git add index.html``` genomför stageing
7. ```git commit --message "Lagt till HTML"```
8. Besvara: Vad rapporterar git?
9. ```git status```
10. ```git log```
11. Notera commit hash typ  `42e95e5b41a4d2351ec2850812b34cf7c2112f11`

---

## Uncommit (återgå till tidigare)

12. Uppdatera ```index.html``` med ```<head>...</head>``` inom ```<html>...</html>```
Stage'a och commit'a ```index.html``` med meddelandet "Lagt till BODY"
13. Tryck "pil upp" för historiska kommandon ```git status```

---

## Git log

14. ```git log```
15. Besvara: Vad visar loggen? Två commits?
16. Notera: commit hash, vilket är tidigare commit?
17. ```git log --stat``` visar förändringar förkortat (pil upp/ned, Q för avslut)
18. ```git log --pretty=oneline``` visar hash, commit message och HEAD
19. ```git log --patch -2``` Visar förändringar i innehållet (pil upp/ned, Q för avslut)

---

## Återställ till tidigare versioner

20. ```git checkout <hash> index.html``` testa att skriva så få hash-tecken som möjligt, börja med första (från vänster)
21. När Git säger ```Prevoious HEAD was <hash>... HEAD is now at <hash>...``` har ny version lästs in
22. ```git status```
23. Besvara: Vad rapporterar git?

---

## Återställ till tidigare versioner

24. Öppna filen ```index.html``` Återställd?
25. Uppdatera ```index.html``` igen med ```<head>...</head> och <body>...</body>``` inom ```<html>...</html>```
Stage'a och commit'a ```index.html``` med meddelandet "Lagt till HEAD och BODY"
26. Bläddra med pil-upp/ned till ```git log -patch -2```  visar innehållet som förändrats (avsluta med CTRL-C)

--- 

(C) Johan Sundström