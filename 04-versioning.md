# 4. Versionshantering

---

## Mål

* States och hantering
* En fils tre tillstånd
* Förflyttning i historiska states

---

## Agenda

* Repository/repo (förråd)
* Snapshots
* Procedur

---

## Versionskontroll

* En mapp eller fil's innehåll kan finnas i olika versioner
* Möjlighet att backa till tidigare versioner

---

## Tänk Snapshots

* Ett snapshot är ett nytt tillstånd
* Ett Repository har flera snapshots av versioner

---

## Tillståndshantering

<img src="https://camo.githubusercontent.com/68c10cf9817f61108313cf3eb561e96913e0f16783a31e344f1414e11dbe41a1/68747470733a2f2f6769742d73636d2e636f6d2f696d616765732f61626f75742f696e646578314032782e706e67">

---

## Stage fil

1. `git add index.html`
2. `git status`
3. Besvara: Vad har filen `index.html` för status (untracked | staged | committed ) och färg?

---

## Unstage fil

4. `git reset index.html` <br>alternativt `git rm --cached index.html`
5. `git status`
6. Besvara: Vad har filen `index.html` för status (untracked | staged | committed ) och färg?
7. `git add index.html` genomför stageing
8. Tryck "pil upp" för historiska kommandon och sänd `git status`

---

## Commit fil

9. `git commit --message "Skapat index.html"`
10. `git status`
11. Besvara: Vad rapporterar git?
12. Editera filen `index.html` med `<head></head>`
13. `git add index.html`
14. `git status`
15. `git commit --message "Lagt till HEAD"`
16. `git status`

---

## Git log

18. `git log`
19. Besvara: Hur många commits?
20. Identifiera: Author, date, commit message
21. Notera: `HEAD -> master` se mer om head i p.27
22. `git log --pretty=oneline` visar hash, commit message och HEAD
23. Notera commit hash typ  `42e95e5b41a4d2351ec2850812b34cf7c2112f11`

---

## Visa innehållsförändringar

24. `git log --stat` visar förändringar förkortat (pil upp/ned, Q för avslut)
25. `git log --patch -2` Visar förändringar i innehållet (pil upp/ned, Q för avslut)

---

## Backa till tidigare state (återgå till tidigare version)

26. `git checkout <hash> index.html` testa att skriva så få hash-tecken som möjligt, börja med första (från vänster)
27. När Git säger `Prevoious HEAD position was <hash>... HEAD is now at <hash>...` har pekare till aktuell state (HEAD) förändrats
28. Öppna filen `index.html` Tidigare version?
29. `git status`
30. Besvara: Vad rapporterar Git?

---

## Flytta HEAD till senaste 

31. `git log` notera senaste hash
32. `git checkout <senaste hash> index.html`
33. Öppna filen `index.html` Återställd till senaste version?

--- 

(C) Johan Sundström