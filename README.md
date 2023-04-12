# Moviium

# Angular10

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 10.1.7.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

kako pokreniti...
api

1. otvoriti Moviium.sln u visual studiu
2. promjeniti putanju do baze u fajlovima MovieContext.cs i appsettings.json
3. pokrenit migracije update-database
4. pokrenit api

angular

1. otvoriti angular10 u visual studio codu
2. promjenit api key... u angular10\src\app\omdb.service.ts private apiURL = 'http://www.omdbapi.com/?apikey={api_key}&';
3. npm install pa ng serve
4. http://localhost:4200/login
