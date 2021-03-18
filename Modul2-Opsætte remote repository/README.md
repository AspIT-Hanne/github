# Modul 2: Oprette remote git repository

I dette modul skal du oprette et remote git repository og forbinde dit lokale repository til det remote. Inden du starter modulet skal du have [oprettet et lokalt repository](https://github.com/AspIT-Hanne/github/tree/master/Modul1-Oprette%20lokalt%20repository).

Du vil efter modulet have kendskab til følgende git kommandoer:
* `remote add`
* `push`
* `pull`
* `status`
* `log`

## Oprette et remote git repository
Du opretter dit remote repository på github.com enten på din forside lige over dine repositories

![Opret nyt repository](https://user-images.githubusercontent.com/57984239/111613334-b12df280-87de-11eb-8cc4-ba1d273f976b.JPG)


... eller inde på din oversigt over alle dine repositories

![Opret nyt repository](https://user-images.githubusercontent.com/57984239/111613339-b25f1f80-87de-11eb-8662-6511212e5ef3.JPG)


På første side skal du give dit repository et navn og vælge, om det skal være public eller private. Hvis det skal være en del af dit online CV, skal det naturligvis være et public repository.

![CreateNewRepo3](https://user-images.githubusercontent.com/57984239/111613343-b3904c80-87de-11eb-9c79-d0aefaab7b32.JPG)


Når du har oprettet dit remote repository og givet det et navn, får du i næste skærmbillede en vejledning til, hvordan du kobler dit lokale repository sammen med dit remote repository.

![Overblik over nyt repository](https://user-images.githubusercontent.com/57984239/111612967-4f6d8880-87de-11eb-8ecb-2861b2dee6b6.JPG)


Da du allerede har oprettet et lokalt repository, skal du kun tilføje det remote site, som du skal tilføje til og lave dit første push.

Det betyder, at du kan bruge den vejledning, der står i afsnittet ".. or push an existing repository from the command line".

## Konfigurer placeringen for dit remote repository

Dit remote site får et alias - det almindeligt anvendte alias er origin. Du kan herefter henvise til "origin" hver gang, du skal henvise til URL'en for dit remote repository.

## Lav dit første push, så du får dine første data op i dit remote repository

`git push -u origin main` "skubber" dine lokale ændringer op til dit remote repository. Origin er alias'et for URL'en for dit remote repository. Master er den branch, du vil pushe ændringer fra. Vi kommer mere ind på branches i en senere opgave.

Argumentet `-u` fortæller `git pull` hvilket remote repository og hvilken branch den skal bruge på efterfølgende pulls. Hvis det ikke sættes nu, så skal man efterfølgende skrive `git pull origin main` hver gang, i stedet for `git pull`, når ændringer skal hentes ned fra remote. 

## Videre herfra
[Opgave: opret og forbind remote repository](https://github.com/AspIT-Hanne/github/blob/master/Modul2-Ops%C3%A6tte%20remote%20repository/opgave17.md)
