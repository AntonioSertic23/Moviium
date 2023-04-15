# Moviium

## Web aplikacija za vođenje evidencije filmova

Izrada stranice Moviium mi je bila dodjeljena kao prvi projekt nakon zaposlenja kako bi stekao znanja u radu sa Anularom i kreiranju API-ja.

Tema projekta je bila napraviti kopiju prijašnje vlastite aplikacije sa faksa "Filmovi" samo u Angularu i sa pripadajućim api-jem za obradu podataka i komunikaciju sa bazom podataka.

Za izradu stranice korišten je **Angular** koji koristi **Bootstrap** za dizajn. Za izradu api-ja korišten je **ASP.NET Core Web API** koji koristi **Swagger** za prikaz kreiranih kontolera. Za bazu podataka korišten je **Microsoft SQL Server**.

[![My Skills](https://skills.thijs.gg/icons?i=angular,bootstrap,dotnet,sqlite)](https://skills.thijs.gg)

Aplikacija sadrži prijavu i registraciju uz potrebne provjere unesenih parametara, a za dohvaćanje filmova i njihovih podataka koristi se [OMDb API](https://www.omdbapi.com/).

---

### Nakon uspješne prijave, u aplikaciji je moguće:

- pretražiti filmove po nazivu
- pogledati detalje pojedinog filma
- dodavanje filmova u svoju listu uz dodjelu vlastite ocjene
- pogledati svoju listu filmova
- ažurirati dodjeljene ocjene
- uklanjanje filmova iz svoje liste

---

### Pokretanje projekta

Prije pokretanja same aplikacije potrebno je pokrenuti API na sljedeći naćin:

1. Otvoriti `Moviium.sln` u Visual Studiu
2. Promjeniti putanje do baze podataka u `MovieContext.cs` i `appsettings.json`
3. Pokreniti migracije na bazu podataka preko `Package Manager Console` gdje pokrećemo sljedeću liniju koda:

```sh
update-database
```

4. Te na kraju pokreniti sami API

Nakon što smo pokrenuli api na red dolazi Angular projekt. Potrebno je

1. Otvoriti `angular10` datoteku u Visual Studio Code-u
2. Kreirati vlastiti _api key_ na službenoj stranici [OMDb API-a](https://www.omdbapi.com/), potom dobiveni _api key_ zalijepiti u `src/app/omdb.service.ts` unutar:

```sh
private apiURL = 'http://www.omdbapi.com/?apikey={api_key}&';
```

3. Pokrenuti komande `npm install` i `ng serve` u terminalu

```sh
npm install
```

```sh
ng serve
```

4. Potom se stranici može pristupiti na: [http://localhost:4200/login](http://localhost:4200/login)
