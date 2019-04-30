# AngularTourOfHeroes

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.3.8.
## Test
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


##Routing
There are new requirements for the Tour of Heroes app:

* Add a Dashboard view.
* Add the ability to navigate between the Heroes and Dashboard views.
* When users click a hero name in either view, navigate to a detail view of the selected hero.
* When users click a deep link in an email, open the detail view for a particular hero.
* When you’re done, users will be able to navigate the app like this:

![Screenshot](nav-diagram.png)


## Summary
1. You added the Angular router to navigate among different components.
2. You turned the AppComponent into a navigation shell with <a> links and a <router-outlet>.
3. You configured the router in an AppRoutingModule
4. You defined simple routes, a redirect route, and a parameterized route.
5. You used the routerLink directive in anchor elements.
6. You refactored a tightly-coupled master/detail view into a routed detail view.
7. You used router link parameters to navigate to the detail view of a user-selected hero.
8. You shared the HeroService among multiple components.
