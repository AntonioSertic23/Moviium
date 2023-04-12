# Moviium

## Angular10

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
2. Kreirati vlastiti _api key_ na službenoj stranici **OMDb API-a**, potom dobiveni _api key_ zalijepiti u `src/app/omdb.service.ts` unutar:

```sh
private apiURL = 'http://www.omdbapi.com/?apikey={api_key}&';
```

3. Pokrenuti komandu `npm install` i `ng serve` u terminalu

```sh
npm install
```

```sh
ng serve
```

4. Potom se stranici može pristupiti na: [http://localhost:4200/login](http://localhost:4200/login)
