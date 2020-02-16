# Introduktion
Materialet i dette repository introducerer til git og GitHub med vejledninger, præsentation og opgaver. Du kommer gennem hvordan du installerer og sætter git op på din computer. Hvordan du laver dit første repository, opretter og tilføjer filer, forpligter dig til ændringer. Du lærer hvordan du kan lægge dit repository på GitHub. Til sidst prøver du at lave en branch.

For at komme igang skal du starte med at installere og opsætte git på din computer.

## For at komme igang

1. Registrer en konto på [GitHub](www.github.com)
2. [Download og installer git](https://git-scm.com/). Under installationen skal der ikke laves om i indstillingerne.
3. Opsæt VS Code til at bruge Git Bash som standard

    3.1 Åben VS Code

    3.2 Vis `Command Palette` (Ctrl + Shift + P)

    3.3 Begynd at skrive `default shell` og vælg kommandoen `Terminal: Select Default Shell` når den kommer frem

    3.4 Vælg `Git Bash`

    3.5 Genstart VS Code

    3.6 Åben din terminal i VS Code (Ctrl + æ) og tjek at den bruger `bash` 
        
    ![Der skal stå bash i øverste højre hjørne i terminalen](./assets/bash-check.png)

    Brug `Bash` i VS Code fordi det virker bedre med copy/paste genveje. Genvejen for for paste er fx Shift + INS i Git Bash uden for VS Code

4. Opsæt git med det rigtige brugernavn og email ved at skrive:
``` bash
$ git config --global user.name "FirstName LastName"
$ git config --global user.email "email@example.com"
```
Dette er vigtigt fordi git bruger disse oplysninger når du arbejder på et projekt.

## Begreber

<dl>
  <dt>Git</dt>
  <dd>Open-source distribueret versionsstyrringssystem. Bruges ofte til, at hndtere ændringer blandt programmører. </dd>
  <dt>Github</dt>
  <dd>Virksomhed der tilbyder gratis hosting af git repositories. Har også tilføjet andre features som bug tracking, feature requests og task management - [Kanban boards](https://en.wikipedia.org/wiki/Kanban_board) - som på Trello</dd>
  <dt>Repository</dt>
  <dd>Det projekt du arbejder på lige nu. Dit repository er lidt firkantet sagt den mappe, hvor alle dine projektfiler ligger i. Et repository kan være enten lokalt (ligge på din computer) eller remote (ligge på en fælles server/sky - fx GitHub)</dd>
  <dt>Clone</dt>
  <dd>En klon af et eksisterende repository. </dd>
  <dt>Origin</dt>
  <dd>Standard navn for det repository, som du opretter på fx GitHub og kloner ned. Det er det remote repository som din klon udspringer fra. Du kan i bund og grund også vælge at kalde URL'en til dit remote repository for "hest" og så skal du bare skrive "hest" hver gang, du vil i kontakt med dit remote repository - fx for at pushe eller pulle.</dd>
  <dt>Remote repository</dt>
  <dd>En online udgave af dit repository. Du arbejder og laver ændringer lokalt i et local repository og pusher derefter dine ændringer til dit remote repository.</dd>
    <dt>Push</dt>
    <dd>At "skubbe" dine filer/ændringer op til et remote repository fra et local repository.</dd>
    <dt>Pull</dt>
    <dd>At "trække" filer/ændringer ned fra et remote repository til dit local repository.</dd>
</dl>


## Videre læsning

[Guide til at skrive gode commit beskeder](https://chris.beams.io/posts/git-commit/)

[GitHub education cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf)

[An interactive git cheat sheet from NPD Software](https://ndpsoftware.com/git-cheatsheet.html)
