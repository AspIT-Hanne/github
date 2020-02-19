# Mere om Issues og Pull Requests

## Forbinde dit Pull Request med det Issue den løser

Hvis du har set videoen fra [Introduktionen til GitHub samarbejde](https://github.com/AspIT-Hanne/github/blob/master/Modul3-GitHub-samarbejde/README.md) har du allerede lært, hvordan man kan forbinde Issues og Pull Requests.
Her kommer vi mere ind på nogle af detaljerne om Issues og Pull Requests, og hvordan vi kan koble dem sammen.

Hvis man har mange Issues i sit repository, kan det være svært at overskue, hvilke Pull Requests der hører sammen med hvilke Issues. Derfor er det vigtigt at få markeret sammenhængen, så man ved, hvilket problem eller hvilken nyudvikling denne Pull Request berører.
Samtidigt giver forbindelsen mellem Issue og Pull Request mulighed for at automatisere nogle arbejdsgange - bl.a. automatisk at få lukket et Issue, når man har accepteret og merged en Pull Request.

Du kan altid henvise til det relevante Issue med et hashtag: #3 henviser til Issue 3.

Du kan bl.a. bruge nogle bestemte keywords til at automatisere lukningen af et Issue, når Pull Requesten er blevet merged. Disse keywords skal skrives i titlen på din Pull Request sammen med hashtag Issuenummer.
Følgende keywords kan bruges til automatisk at lukke et Issue:

* close
* closes
* closed
* fix
* fixes
* fixed
* resolve
* resolves
* resolved

En god titel på en `pull request` kunne være:

Fixes #2 - Change colorscheme on contact page

[Læs mere om at linke et pull request til et bestemt issue her](https://help.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue)

## Reviewe et Pull Request

Når du har lavet et Pull Request, kan du bede andre om at gennemse det, komme med ændringsforslag, kommentere eller godkende dit Pull Request.

Når du har dit Pull Request åbent, kan du i den højre kolonne øverst klikke på tandhjulet til højre for `Reviewers` og skrive brugernavnet på den person, du gerne vil have til at reviewe dit Pull Request.
Du kan også tilføje flere reviewers til et Pull Request.

Når man er blevet bedt om at reviewe et Pull Request, får man en gul linje over Pull Request detaljerne, hvis man er blevet bedt om at reviewe det.

I den gule linje er der to knapper: en til at se ændringsforslagene lokalt (hvis du fx. gerne vil se i en browser eller i din kodeeditor, hvordan ændringerne ser ud) og en til at reviewe Pull Requesten.

### Previewe ændringsforslaget fra dit lokale repository - fx i en kodeeditor eller browser

Hvis du klikker på `Check out locally` kommer der tre linjers kode frem, hvis du står under punktet `Git`. Du kan klikke på knappen til højre (clipboardet), og så bliver de tre linjers kode kopieret.

![GitHub-check-pull-request-locally](https://user-images.githubusercontent.com/57984239/74838719-577d9f00-5324-11ea-8e15-516c1eff8b0a.JPG)

Herefter går du ind i din kodeeditor (fx VS Code) og indsætter den kopierede kode. Din kodeeditor vil nu hente de nyeste opdateringer (bl.a. den udviklingsbranch, som Pull Requesten er baseret på), skifte til den udviklingsbranch og merge den sammen med dit lokale repository.

Du kan nu previewe den foreslåede kode i en browser.

### Reviewe, kommentere, foreslå ændringer og godkende Pull Requests

Hvis du klikker på den grønne "Add your review"-knap, når du står inde i en Pull Request, kommer du videre til fanebladet `Files changed`.
Her kan du se de forskelle, der er på koden i master branchen og koden i udviklingsbranchen, som Pull Requesten kommer fra.

Under den grønne Review-knap findes der et vindue, hvor du kan reagere på tre forskellige måder: kommentere, foreslå ændringer eller godkende Pull Requesten.

![GitHub-review](https://user-images.githubusercontent.com/57984239/74839129-09b56680-5325-11ea-8b8c-d862e1fb113d.JPG)

Hvis du skriver her, vil du efterlade et generelt review af Pull Requesten, som alle kan se i Pull Requestens `Conversation` faneblad.

Du kan også lave en mere specifik kommentar på en bestemt kodelinje: Hvis du placerer din markør til højre for kodelinjen, kommer der et blåt kryds frem, som du kan trykke på. Det åbner en boks, hvor du kan skrive din kommentar. Dette bliver også tilgængeligt for alle i `Conversation` fanebladet.


![GitHub-review-single-line-comment](https://user-images.githubusercontent.com/57984239/74839679-f6ef6180-5325-11ea-8a8e-54b4ef47a842.JPG)

Det er vigtigt, at du er ærlig i dine reviews på en konstruktiv måde. Hvis du arbejder på et repository sammen med fx kolleger, som fysisk er placeret samme sted som dig, kan man ofte snakke om eventuelle misforståelser og uklarheder med det samme. Men samarbejder man med andre online er det vigtigt, at være utrolig præcis i sit review og at være konstruktiv og positiv, når man giver sin ærlige mening - især hvis der er noget, man ikke synes er løst på en specielt god måde.

Nedenfor kan du se et eksempel på en Conversation i et Pull Request:

![GitHub-review-conversation](https://user-images.githubusercontent.com/57984239/74840026-914fa500-5326-11ea-91f1-65bbdce1e670.JPG)
