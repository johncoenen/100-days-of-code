### Personal Log 

### Monday, January 1, 2018

**Today's Progress**: 
  Created a basic ASP.NET MVC app
  
**Thoughts** 
  - Nice to revisit Visual Studio after some time away
  - Learned the basic fundamentals that go into creating a MVC application
  - Understand how Views are created and manipulated within the ASP.NET stack
  
**Link(s)**

https://github.com/johncoenen/ASP.NET-MVC---Basic-Template

### Tuesday, January 2, 2018

**Today's Progress**: 
  Created a basic responsive web app with HTML5 and CSS Media Queries(from demo)
  
**Thoughts** 
  - Quick and dirty project
  - Using HTML5 semantics and media queries
  - First time really using Emmet shorthand in VSCode!
  - TODO: fix issues with font awesome icons, change styling/markup to be more accessible
  
**Link(s)**
https://github.com/johncoenen/QuickApps/tree/master/ResponsiveApp_HTML5_CSS

### Wednesday, January 3, 2018

**Today's Progress**: 
  Begin looking at jQuery UI, starting with draggable DOM elements
  
**Thoughts** 
  - Easy to user interface
  - Less javascript than expected
  - First time really using jQuery  
  
**Link(s)**
https://github.com/johncoenen/jQuery

### Thursday, January 4, 2018

**Today's Progress**: 
  Finished DOM tutorial called Understanding the DOM
  
**Thoughts** 
  - Most of the work was done in the dev tools console so I will just link to the article
  - Introduction to the DOM
  - DOM trees and nodes
  - Access elements in the DOM
  - Traverse the DOM
  - Change elements in the DOM
  
**Link(s) to work**
https://www.digitalocean.com/community/tutorial_series/understanding-the-dom-document-object-model

### Friday, January 5, 2018

**Today's Progress**: 
  Began HTML Forms tutorial, with emphasis on how screen readers interpret forms
  
**Thoughts** 
  - Looked at how screen readers order the elements of a form
  - Learned best practices for required field form elements
  
**Link(s)**
https://github.com/johncoenen/HTML/tree/master/forms-screen_reader

### Sat/Sun, January 6/7, 2018

**Today's Progress**: 
  Continue HTML forms tutorials looking at payment form and formfield input widgets

**Thoughts** 
  - Built a payment form
  - Tested checkboxes, radio buttons, submit, reset, anonymous buttons, etc...
  
**Link(s)**
https://github.com/johncoenen/HTML/tree/master/payment-form
https://github.com/johncoenen/HTML/tree/master/form-fields

### Monday, January 8, 2018

**Today's Progress**: 
  Build ASP.NET Core Angular application from tutorial
  
**Thoughts** 
  - It's a miracle this works at all, but I will call this a win
  - The tutorial was well written and I only had a few workarounds and bugs to deal with
  - First time getting an Angular app running with Visual Studio 2017
  - Will be continuing this tutorial tomorrow and adding enhancments  
  
**Link(s)**
tutorial: https://medium.com/@levifuller/building-an-angular-application-with-asp-net-core-in-visual-studio-2017-visualized-f4b163830eaa
working demo: https://github.com/johncoenen/ASP.NET-Angular-Starter

### Wednesday, January 10, 2018

**Today's Progress**: 
  Added developer-friendly enhancements to ASP.NET Core Angular app
  
**Thoughts** 
  - Proxy API calls to the ASP.NET Core Server using ng serve command
    -- this watches for changes to the code, transpiles the code, and reserves the code to localhost:4200 by default
  - Enabled automatic re-compilation for ASP.NET Core
    -- enables the ability to make changes to (server-side)code and show live changes in the already running Angular app
  - In order to run both applications in watch mode:
    -- First run: dotnet watch run (command)
    -- Then run: ng serve --proxy-config proxy.config.json(command in another terminal)
    -- Then browse to localhost:4200(default) to see live changes made to app

**Link(s)**
tutorial: https://medium.com/@levifuller/building-an-angular-application-with-asp-net-core-in-visual-studio-2017-visualized-f4b163830eaa
1/10/2018 demo: https://github.com/johncoenen/ASP.NET-Angular-Starter 

### Thursday, January 11, 2018

**Today's Progress**: 
  - Begin Angular Tutorial: Tour of Heroes
  - complete steps 1 - 4 of tutorial
    -- This app is data-driven and will enable the user to:
      1. display a list of hero names
      2. edit selected hero's details
      3. navigate through different views of the hero's data
    - Created the application shell which consists of a html, css, and typescript file
      - created initial structure using Angular CLI
      - learned Angular components display data
      - used double curly braces syntax to display the app title
    - Created the Hero Editor
      - used the CLI to create a second HeroesComponent
      - displayed the HeroesComponent by adding it to the AppComponent shell.
      - applied the UppercasePipe to format the name
      - used two-way data binding with the ngModel directive
      - learned about the AppModule
      - imported the FormsModule in the AppModule so that Angular would recognize and apply the ngModel directive
      - learned the importance of declaring components in the AppModule  
    - Created a display for Hereos List
      - The Tour of Heroes app displays a list of heroes in a Master/Detail view.
      - The user can select a hero and see that hero's details.
      - used *ngFor to display a list
      - used *ngIf to conditionally include or exclude a block of HTML
      - learned to toggle a CSS style class with a class binding
  
**Link(s)**
tutorial: https://angular.io/tutorial (Tour of Heroes)
demo: https://github.com/johncoenen/Angular-Tour-Of-Heroes

### Saturday, January 13, 2018

**Today's Progress**: 
  - (cont.)Angular Tour of Heros
    - Created a separate, reusable HeroDetailComponent
    - Used property binding
      - this gives the parent HeroesComponent control over the child HeroDetailComponent
    - Used the @Input decorator
      - this makes the hero property available for binding by the external HeroesComponent
  
**Thoughts** 
  - After this post I am going to begin implementing some small changes to the daily log format
    - These are my notes for the areas that will remain/change:
      - Keep timestamp for day, date, year
        - add time spent per day using time tracking app
      - (maybe) change Thoughts area to include more information on the days lesson
        - more blog-like, where I will take the most important detail of the day and expand on the terminology 
      - Add another category where tech detail links can be added 

### Monday, January 15, 2018

**Today's Progress**: 
  - (cont.)Angular Tour of Heros
    - Dipped into Angular Dependency Injection 
    - added get data method to HeroService which is an asynchronous signature
    - Used Observable and the RxJs Observable libray
    - Used RxJs of() to return Observable of mock heroes ( Observable<Hero[]> )
    - The component's ngOnInit lifecycle hook calls the HeroService method, not the constructor.
    - You created a MessageService for loosely-coupled communication between classes.
    - The HeroService injected into a component is created with another injected service, MessageService.

**Thoughts** 
  - still have to implement some changes in this structre, may wait til next project
  - 1:01 - time spent on Services portion of this 
  - This is one of the more important sections of the Tutorial. I am going to go back to the beginning
    and write down the important areas of interest, up to this point, as a personal reference

**Link(s)**
https://github.com/johncoenen/Angular-Tour-Of-Heroes 

### Tuesday, January 16, 2018

**Today's Progress**:
  - Started a project currated by Sarah Drasner called Creating a Vue.js Serverless Checkout Form: Setup and Testing. 
  - Set up Azure and Stripe accounts
  - Configured basic serverless funciton application using Azure
  - set up application architecture using node and npm

**Thoughts**
  - Straight forward and easy to follow tutorial with code examples made getting started a breeze

**Link(s)**
https://css-tricks.com/creating-vue-js-serverless-checkout-part-one/

## Thursday, January 18, 2018

**Today's Progress**:
  - Continued on Vue.js-Azure-Stripe project
  - Started working on part 2 of this series titled Creating a Vue.js Serverless Checkout Form: Stripe Function and Hosting.
  - Couldn't get this to work properly and will have to come back once the other parts of the series are published.
  - Something is not configured correctly btwn. Azure and Stripe, testing confirms some errors, but have yet to resolve these
  
## Friday, January 19, 2018

**Today's Progress**:
  - Revisiting jQuery, which I haven't used in awhile
  - I am aware that jQuery is going out of style. In order to understand how Javascript(ES6) is being used to recreate this functionality, I feel I need to know how jQuery works.
  - At the moment I am just going through the w3c website completing the small built in tutorials
  
## Saturday/Sunday, January 20/21, 2018

**Today's Progress**:
- Began the Wes Bos course on CSS Grid this weekend
- Worked through 1 - 9 of the videos

**Thoughts**
- I have completed two other courses by Wes Bos and like the way he presents the overlying concepts
- Really enjoy CSS Grid and was happy to dig in again 
- Nice to finally use the Firefox dev tooling created for Grid

**Links(s)**
Link to free course:  https://cssgrid.io/
Link to my work: https://github.com/johncoenen/CSS-Grid-with-Wes-Bos-Coursework

## Wednesday, January 24, 2018

**Today's Progress**:
- Worked through the Routing portion of the Angular Tour of Heroes tutorial

**Thoughts**
- Added the Angular router to navigate among different components.
- Turned the AppComponent into a navigation shell with <a> links and a <router-outlet>.
- Configured the router in an AppRoutingModule
- Defined simple routes, a redirect route, and a parameterized route.
- Used the routerLink directive in anchor elements.
- Refactored a tightly-coupled master/detail view into a routed detail view.
- Used router link parameters to navigate to the detail view of a user-selected hero.
- Shared the HeroService among multiple components.

## Saturday, January 27, 2018

**Today's Progress**:
- Worked through the Http portion of the Angular Tour of Heroes tutorial
- Finished the Tour of Heroes tutorial and completed the application!

**Thoughts**
- Added the necessary dependencies to use HTTP in the app.
- Refactored HeroService to load heroes from a web API.
- Extended HeroService to support post(), put(), and delete() methods.
- Updated the components to allow adding, editing, and deleting of heroes.
- Configured an in-memory web API.
- Learned how to use Observables.

**Link(s)**
https://github.com/johncoenen/Angular-Tour-Of-Heroes





