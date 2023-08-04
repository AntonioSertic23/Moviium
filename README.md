# Moviium

## Web application for managing movie records

The creation of the Moviium website was assigned to me as my first project after employment to gain knowledge in working with Angular and creating APIs.

The project's theme was to make a copy of my previous custom application from college called [Movies](https://github.com/AntonioSertic23/Movies) but this time using Angular and a corresponding API for data processing and communication with the database.

The website was built using **Angular**, which utilizes **Bootstrap** for design. For creating the API, **ASP.NET Core Web API** was used, and **Swagger** was used to display the created controllers. The **Microsoft SQL Server** was used as the database.

[![My Skills](https://skills.thijs.gg/icons?i=angular,bootstrap,dotnet,sqlite)](https://skills.thijs.gg)

The application includes login and registration with necessary parameter checks. To fetch movies and their data, the [OMDb API](https://www.omdbapi.com/) is used.

---

### After successful login, the application allows you to:

- Search for movies by title
- View details of a specific movie
- Add movies to your own list along with a personal rating
- View your list of movies
- Update assigned ratings
- Remove movies from your list

---

### Running the project

Before running the application itself, you need to start the API as follows:

1. Open `Moviium.sln` in Visual Studio
2. Change the database paths in `MovieContext.cs` and `appsettings.json`
3. Run migrations on the database via the `Package Manager Console` by executing the following line of code:

```sh
update-database
```

4. Finally, run the API itself

Once the API is running, it's time to start the Angular project. Follow these steps:

1. Open the `angular10` folder in Visual Studio Code
1. Create your own _api key_ on the official [OMDb API](https://www.omdbapi.com/) website, then paste the obtained _api key_ inside `src/app/omdb.service.ts` within the following line:

```sh
private apiURL = 'http://www.omdbapi.com/?apikey={api_key}&';
```

3. Execute the commands `npm install` and `ng serve` in the terminal

```sh
npm install
```

```sh
ng serve
```

4. Access the website at: [http://localhost:4200/login](http://localhost:4200/login)
