# 1. Koncept

---

## Mål

* Få övergripande förståelse för Git
* Kunna skilja på Git och Github

---

## Vanans makt

* Ute - spara filversioner
* Inne - spara states (tillstånd)

---

## Problemet med filversioner

* Filuppdateringar leder till filversioner
* Filhistorik blir svårhanterlig, vilken är aktuell?
* Samarbete med filer omöjligt
* Distribution av filer krävande

---

## Lösningen med Tillståndsversioner

* Färdigutvecklade delar sparas
* Medarbetare förstår generationer av färdiga delar bättre

---

## 1. Vad är Git?

<img src="https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png" width="10%" height="10%" />

* Utvecklingen av Linux och dess distrubution krävde versionshanteringsprogram
* _Git_ är ett versionshanteringsprogram VCS (Version Control System), _Subversion_ (SVN) är andra
* _Git_ är inte filversioner
* Versionshantering innebär stöd för _traceability_, möjligheten att backa till tidigare versioner

---

## 1. Vad är Git?

<img src="https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png" width="10%" height="10%" />

* Stödjer flera användare i ett team eller projekt genom branch-based workflow (_branching_ och _merging_)
* Är de facto _standard_ och benämns vara _lightwheight_
* _Open source_, skapat av Linus Thorvalds 2005
* Lanserades 10 april 2008 (wiki)

---

## 2. Vad är Github?

<img src="https://github.githubassets.com/images/modules/logos_page/Octocat.png" width="10%" height="10%" />

* Hosting platform för versionskontroll, samarbete men främst distribution
* 56 miljoner användare (Sept 2020 - Wiki)
* Git är ett kommandoradsverktyg
* Github är hubben (navet) för Git på webben
* Github är lagringsplatsen

---

## 3. Version Control Systems

* Centraliserade - SPOF
* Distribuerade - Synkningar sker mellan användare

--- 

(C) Johan Sundström