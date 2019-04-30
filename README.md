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


## Services
The Tour of Heroes HeroesComponent is currently getting and displaying fake data.

After the refactoring in this tutorial, HeroesComponent will be lean and focused on supporting the view. It will also be easier to unit-test with a mock service.

## Why services
Components shouldn't fetch or save data directly and they certainly shouldn't knowingly present fake data. They should focus on presenting data and delegate data access to a service.

In this tutorial, you'll create a HeroService that all application classes can use to get heroes. Instead of creating that service with new, you'll rely on Angular dependency injection to inject it into the HeroesComponent constructor.

Services are a great way to share information among classes that don't know each other. You'll create a MessageService and inject it in two places:

1. in HeroService which uses the service to send a message.
2. in MessagesComponent which displays that message.

## Summary
1. You refactored data access to the HeroService class.
2. You registered the HeroService as the provider of its service at the root level so that it can be injected anywhere in the app.
3. You used Angular Dependency Injection to inject it into a component.
4. You gave the HeroService get data method an asynchronous signature.
5. You discovered Observable and the RxJS Observable library.
6. You used RxJS of() to return an observable of mock heroes (Observable<Hero[]>).
7. The component's ngOnInit lifecycle hook calls the HeroService method, not the constructor.
8. You created a MessageService for loosely-coupled communication between classes.
9. The HeroService injected into a component is created with another injected service, MessageService.
