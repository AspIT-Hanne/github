# Oprette remote repository

I denne opgave skal du oprette et remote repository på GitHub

For at kunne lave opgaven skal du på forhånd have [installeret og sat git op på din computer](https://github.com/AspIT-Hanne/github#for-at-komme-igang) og [oprettet et lokalt repository](https://github.com/AspIT-Hanne/github/tree/master/Modul1-Oprette%20lokalt%20repository)


## Opgaven

Brug GitHub til at oprette et nyt tomt repository kaldet hello-git. Herefter skal du bruge de kommandoer, som GitHub selv giver dig umiddelbart efter oprettelsen, til at forbinde dit lokale repository med det nye remote repository. 

Når du har løst opgaven skal du tage et screenshot af de kommandoer du har skrevet i din terminal og sende det til din lærer.

Hints:
* `git remote add` - tilføjer et remote repository med et navn. Konventionen er at navnet er origin.
* `git push` Opdaterer remote repository med lokale ændringer. `-u` eller `--set-upstream` fortæller `git pull` hvilket remote repository og hvilken branch den skal bruge på efterfølgende pulls. His det ikke sættes nu så skal man efterfølgende skrive `git pull origin master` hver gang, i stedet for `git pull`, når ændringer skal hentes ned fra remote. Når du først har lavet en -u behøver du ikke længere skrive hvilket remote repository, du vil pushe til og hvilken branch, du pusher fra/til. 

