# Oprette lokalt repository

I denne opgave skal du oprette et lokalt git repository ved at bruge terminal.

For at kunne lave opgaven skal du på forhånd have [installeret og sat git op på din computer](https://github.com/Visualisering-DK/github/blob/master/README.md#for-at-komme-igang).


## Opgave 1

Start med at oprette en lokal mappe og lav den til et git repository. Herefter skal du oprette en fil kaldet README.md. Filen skal trackes af dit git repository og efterfølgende skal den committes til et snapshot af dens nuværende tilstand. Hele opgaven skal laves i en terminal. 

Når du har løst opgaven skal du tage et screenshot af de kommandoer du har skrevet og sende det til din lærer på mail (halu@aspit.dk).

Hints:
* `mkdir` opretter mapper (make directory)
* `cd` ændrer mappen du er i (change directory). Fx `cd minMappe/` går ind i mappen 'minMappe'. Hvis du vil gå et niveau op skrives `cd ..`
* `touch` opretter filer (rører en fil. Hvis filen ikke eksisterer oprettes den)

## Opgave 2

Når du er færdig med at oprette det lokale repository i opgaven, skal du oprette et lokalt repository med din V-relaterede kode i.
Åbn din terminal og sørg for at du står i V1-mappen. Du kan se, hvilken mappe, du er i ved at skrive `pwd` (print working directory). Hvis du skal skifte mappe, kan du gøre det med `cd [mappenavn]` for at gå ned i en mappe og `cd..` for at gå ud af en mappe og et niveau op.

Opret dit nye lokale V1-repository ved at skrive `git init`, mens du står i V1-mappen i terminalen.

## Hvis du allerede har filer liggende i fx din V1-mappe
Sørg for at flytte dine filer fra dit Working Directory til dit Staging Area med `git add .` (eller filnavn). Sørg herefter for at flytte dine stagede filer fra staging area til det lokale repository vha `git commit -m "commit besked"`.
