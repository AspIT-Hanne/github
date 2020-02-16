# Modul 3 - GitHub samarbejde

I dette modul lærer du, hvordan du kan bruge GitHub til at samarbejde med andre om et projekt via et fælles remote repository.

Du lærer også, hvordan du opretter og arbejder på branches.

## Arbejde med branches

Hvis du eksperimenterer med nye funktioner eller features på dit projekt, kan du køre disse ændringer i et sideløbende spor (en sideløbende branch), så det ikke påvirker dit nuværende fungerende projekt.

Dit publicerede, kørende projekt ligger i en Master Branch. Hvis du vil lave et sideløbende eksperimentelt spor, kan du oprette en ny branch, lave dine ændringer, stage, committe og pushe dem. Dette påvirker ikke din Master Branch.

Med kommandoen `git branch` kan du se alle de branches, som du har i dit projekt på nuværende tidspunkt

```bash
halu@CV-BB-5984 MINGW64 ~/code/Git-cooperation (master)
$ git branch
* master
```

Asterisken/stjernen ved siden af branch navnet angiver hvilken branch, du arbejder på på nuværende tidspunkt. Alle dine commits bliver lavet under denne branch.
Du kan også se i linjen med dit brugernavn, at du arbejder på branchen "master". Dette er angivet i parentes sidst i den linje.

Git gemmer også den branch, du sidst har committed i under keywordet HEAD. Hvis du vil se, hvad din HEAD er på nuværende tidspunkt, kan du bruge kommandoen `git show-ref --head`.

```bash
halu@CV-BB-5984 MINGW64 ~/code/Git-cooperation (master)
$ git show-ref --head
3d53d36c2ac79c22f4d3dda30fd9e06551540e16 HEAD
3d53d36c2ac79c22f4d3dda30fd9e06551540e16 refs/heads/master
3d53d36c2ac79c22f4d3dda30fd9e06551540e16 refs/remotes/origin3/master
```

Du vil så se, at hvis du sidst har committed på din Master Branch, henviser head til den. Du kan se det samme, hvis du bruger `git log`

```bash
halu@CV-BB-5984 MINGW64 ~/code/Git-cooperation (master)
$ git log
commit 3d53d36c2ac79c22f4d3dda30fd9e06551540e16 (HEAD -> master, origin3/master)
Author: Hanne <57984239+AspIT-Hanne@users.noreply.github.com>
Date:   Sun Feb 16 16:32:44 2020 +0100

    Create Opgave16Github-samarbejde.md
```

Du opretter en ny branch med kommandoen `git branch [navn på ny branch]`.

Du skifter over til en anden branch med kommandoen `git checkout [navn på branch du vil skifte til]`.

Næste gang du committer vil det blive til den branch, du er skiftet til. Er du i tvivl om, hvilken branch du arbejder med, kan du altid kontrollere det med `git branch`.

## Issues og pull requests

Når du arbejder på et projekt/remote repository med andre, kan der oprettes issues. Et issue er en ændring, som nogen gerne vil have lavet i projektet, og som de derfor lægger ud til, at man kan melde ind på at løse issuet.

Issues oprettes på github.com.

Hvis du tager et issue og vælger at arbejde på det, skal du oprette en ny branch til dit arbejde, så du ikke kommer til at pushe ændringer i master branchen.

Når du er færdig med dine ændringer stager, committer og pusher du ændringerne fra din nye branch til det remote repository.

Du laver herefter et `pull request` på github.com på dine ændringer. Du beder om, at dine ændringer fra din branch, bliver "pull'et" ind og merged (flettet sammen med) master branchen.

Når du laver din `pull request` henviser du til det Issue (med #[Issuenummer] - fx #3 hvis du arbejder på issue 3).

Når du har lavet et `pull request`, kan dine samarbejdspartnere/kolleger kommentere på dine ændringer, og hvis projektejeren synes, at ændringerne kan bruges, kan han/hun acceptere `pull request'en` og `merge` dine branch ind i master branchen.

Projektlederen kan herefter lukke det Issue, som din løsning fixede og slette din udviklings branch.

Det er altid en god idé at slette udviklings branches, når de ikke længere skal bruges, så de ikke bidrager til forvirring efterhånden som der kommer flere og flere udviklingsbranches.
