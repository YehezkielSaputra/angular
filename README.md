# Angular

## Table of Contents

### 1. Angular Basics 

| No. |   Questions                                              |
|-----|----------------------------------------------------------|
| 01. |[What is an Angular Module?](#q-what-is-an-angular-module)|
| 02. |[What are the case types in Angular?](#q-what-are-the-case-types-in-angular)|
| 03. |[What is the difference between AngularJS and Angular?](#q-what-is-the-difference-between-angularjs-and-angular)|
| 04. |[What are the frequently used command in angular?](#q-what-are-the-frequently-used-command-in-angular)|
| 05. |[What are lifecycle hooks available in Angular?](#q-what-are-lifecycle-hooks-available-in-angular)|
| 06. |[What is data binding in Angular?](#q-what-is-data-binding-in-angular)|
| 07. |[What is the difference between constructor() and ngOnInit()?](#q-what-is-the-difference-between-constructor-and-ngoninit)|
| 08. |[What are Angular Services?](#q-what-are-angular-services)|
| 09. |[What is Interpolation?](#q-what-is-interpolation)|
| 10. |[What is index property in ngFor directive?](#q-what-is-index-property-in-ngfor-directive)|
| 11. |[What happens if you use script tag inside template?](#q-what-happens-if-you-use-script-tag-inside-template)|
| 12. |[What are template expressions?](#q-what-are-template-expressions)|
| 13. |[What are template statement?](#q-what-are-template-statement)|
| 14. |[How do you enable binding expression validation?](#q-how-do-you-enable-binding-expression-validation)|
| 15. |[What is the purpose of any type cast function?](#q-what-is-the-purpose-of-any-type-cast-function)|
| 16. |[What is Non null type assertion operator?](#q-what-is-non-null-type-assertion-operator)|
| 17. |[How do you describe various dependencies in angular application?](#q-how-do-you-describe-various-dependencies-in-angular-application)|
| 18. |[What is declarable in Angular?](#q-what-is-declarable-in-angular)|
| 19. |[What are the restrictions on declarable classes?](#q-what-are-the-restrictions-on-declarable-classes)|
| 20. |[When to use NgOnInit and constructor in Angular?](#q-when-to-use-ngoninit-and-constructor-in-angular)|
| 21. |[What is the expression context in Angular?](#q-what-is-the-expression-context-in-angular)|
| 22. |[How can you add an active class to a selected element in a list component?](#q-how-can-you-add-an-active-class-to-a-selected-element-in-a-list-component)|
| 23. |[What is the purpose of NgModule? How do you decide to create a new NgModule?](#q-what-is-the-purpose-of-ngmodule-how-do-you-decide-to-create-a-new-ngmodule)|
| 24. |[What is difference between Angular Modules and JavaScript Modules?](#q-what-is-difference-between-angular-modules-and-javascript-modules)|
| 25. |[How would you make use of ngOnInit()?](#q-how-would-you-make-use-of-ngoninit)|


#### Q. ***What is an Angular Module?***
In Angular, a module is a mechanism to group components, directives, pipes and services that are related, in such a way that can be combined with other modules to create an application. 

```typescript
import { NgModule }      from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent }  from './app.component';

@NgModule ({
    imports:      [ BrowserModule ],
    declarations: [ AppComponent ],
    bootstrap:    [ AppComponent ]
})
export class AppModule { }
```
The NgModule decorator has three options
* The imports option is used to import other dependent modules. The BrowserModule is required by default for any web based angular application
* The declarations option is used to define components in the respective module
* The bootstrap option tells Angular which Component to bootstrap in the application
