# Why Angular 2

There are many different front-end JavaScript frameworks to choose from today.
Each framework comes with its own set of trade-offs.
Many people and organizations were happy with the functionality that Angular 1.x afforded them.
Angular 2 takes all of that Angular 1.x functionality and improves on it by being faster, more scalable, and more modern.
Chances are that organizations that found value in Angular 1.x will find more value in Angular 2.

## Angular 2's Advantages

When Angular was first released, it provided developers with the tools to develop and architect large scale JavaScript applications; its age has revealed a number of flaws and sharp edges.
Angular 2 has been designed to build on the last five years of community feedback.

### Angular 2 Is Easier

Years of feedback have made Angular 2 more modern, more capable, and easier for new developers to learn than Angular 1.x.
In turn Angular 2 is also easier for project veterans to work with.
Ultimately this makes for a codebase that's all around easier for everyone to deal with.

With Angular 1, one had to keep in mind and understand the differences between Controllers, Services, Factories, Providers and other concepts that could be confusing, especially for new developers.
Angular 2 is a more streamlined framework that allows developers to focus on simply building JavaScript classes.

In Angular 2, views and controllers are gone and replaced with components, which can be described as a refined version of directives.
Even experienced Angular developers are not always aware of all the capabilities of Angular 1.x directives.
Angular 2 components are considerably easier to read, and their API features less jargon than Angular 1.x's directives.
Additionally to help ease the transition to Angular 2, the Angular team has added a `.component` method to Angular 1.5, which has been [back-ported by community member Todd Motto to v1.3](https://toddmotto.com/angular-component-method-back-ported-to-1.3/).

### TypeScript

Angular 2 was written in TypeScript, a superset of JavaScript that implements many up and coming ES2016+ features.

By focusing on making their framework easier for computers to process, Angular 2 allows for a much richer development ecosystem.
Developers using sophisticated text editors (or IDEs) will notice dramatic improvements with auto-completion and type suggestions.
These improvements in tooling can help reduce the cognitive burden of learning Angular 2.
Fortunately for traditional ES5 JavaScript developers this does *not* mean that development must be done in TypeScript or ES2015.
Developers are still able to write vanilla JavaScript that runs without transpilation.

### Familiarity

Despite being a complete rewrite, Angular 2 still shares many of its core concepts and conventions with Angular 1.x, e.g. a streamlined, "native JS" implementation of dependency injection.
This means that developers who are already proficient with Angular will have an easier time migrating to Angular 2 than another library like React or framework like Ember.

### Performance and Mobile

Mobile use of the web is huge and growing.
Mobile devices keep getting more powerful, but they're still quite under-powered when compared to a modern desktop; smartphones typically also have less data bandwidth to work with.

Angular 2 was designed for mobile from the ground up.
Aside from limited processing power, mobile devices have other features and limitations that separate them from traditional computers.
Touch interfaces, limited screen real estate, and mobile hardware have all been considered in Angular 2.

The nature of computing performance means that desktops will also see "dramatic" improvements in performance and responsiveness.
Early benchmarks performed on Angular 2 alpha confirm that "dramatic" is an accurate choice of word.
Note that benchmarks are tricky to get right, and even when done correctly can be misleading. Nevertheless Angular 2 *alpha*'s rendering performance vs Angular 1.4's is astounding at scale.

Angular 2, like React and other modern frameworks, can leverage performance gains by rendering HTML on the server or even in a web worker.
Depending on application/site design this isomorphic rendering can make a user's experience *feel* even more instantaneous.

The quest for performance does not end with pre-rendering.
Angular 2 makes itself portable to native mobile by integrating with [NativeScript](https://www.nativescript.org/), an open source library that bridges JavaScript and mobile.
Additionally, the Ionic team is working on an Angular 2 version of their product, providing *another* way to leverage native device features with Angular 2.

### Project Architecture and Maintenance

The first iteration of Angular provided web developers with a highly flexible framework for developing applications.
This was a dramatic shift for many web developers, and while that framework was helpful, it became evident that it was often too flexible.
Over time, best practices evolved, and a community community-driven structure was endorsed.

Angular 1.x tried to work around various browser limitations related to JavaScript.
This was done by introducing a module system that made use of dependency injection. This system was novel, but unfortunately had issues with tooling, notably minification and static analysis.
Angular 2.x makes use of the upcoming ES2015 module system, and modern packaging tools like Webpack or SystemJS.

With Angular 2, modules are far less coupled to the "Angular way", and it's easier to write more generic JavaScript and plug it into Angular.
The removal of minification workarounds and the addition of rigid prescriptions make maintaining existing applications simpler.
The new module system also makes it easier to develop effective tooling that can reason better about larger projects.

### New Features

Some of the other interesting features in Angular 2 are:

- Form Builder
- Change Detection
- Templating
- Routing
- Annotations
- Observables
- Shadow DOM

## Differences Between Angular 1 & 2
> Note that "Transitional Architecture" refers to a style of Angular 1 application written in a way that mimics Angular 2's component style, but with controllers and directives instead of TypeScript classes.

| Old School Angular 1.x | Angular 1.x Best Practices | **Transitional Architecture**             | Angular 2
--------------------------------------|------------------------| ---------------------------|------------------------------|----------------------
Nested scopes ("$scope", watches)     | Used heavily           | Avoided                    | **Avoided**                  | Gone
Directives vs controllers             | Use as alternatives    | Used together              | **Directives as components** | Component directives
Controller and service implementation | Functions              | Functions                  | **ES6 classes**              | ES6 classes
Module system                         | Angular's modules      | Angular's modules          | **ES6 modules**              | ES6 modules
Requires a transpiler                 | No                     | No                         | **TypeScript**               | TypeScript