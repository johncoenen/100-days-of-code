## Personal Log 

## Monday, January 1, 2018

**Today's Progress**: 
  Created a basic ASP.NET MVC app
  
**Thoughts** 
  - Nice to revisit Visual Studio after some time away
  - Learned the basic fundamentals that go into creating a MVC application
  - Understand how Views are created and manipulated within the ASP.NET stack
  
**Link(s)**

https://github.com/johncoenen/ASP.NET-MVC---Basic-Template

## Tuesday, January 2, 2018

**Today's Progress**: 
  Created a basic responsive web app with HTML5 and CSS Media Queries(from demo)
  
**Thoughts** 
  - Quick and dirty project
  - Using HTML5 semantics and media queries
  - First time really using Emmet shorthand in VSCode!
  - TODO: fix issues with font awesome icons, change styling/markup to be more accessible
  
**Link(s)**
https://github.com/johncoenen/QuickApps/tree/master/ResponsiveApp_HTML5_CSS

## Wednesday, January 3, 2018

**Today's Progress**: 
  Begin looking at jQuery UI, starting with draggable DOM elements
  
**Thoughts** 
  - Easy to user interface
  - Less javascript than expected
  - First time really using jQuery  
  
**Link(s)**
https://github.com/johncoenen/jQuery

## Thursday, January 4, 2018

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

## Friday, January 5, 2018

**Today's Progress**: 
  Began HTML Forms tutorial, with emphasis on how screen readers interpret forms
  
**Thoughts** 
  - Looked at how screen readers order the elements of a form
  - Learned best practices for required field form elements
  
**Link(s)**
https://github.com/johncoenen/HTML/tree/master/forms-screen_reader

## Sat/Sun, January 6/7, 2018

**Today's Progress**: 
  Continue HTML forms tutorials looking at payment form and formfield input widgets

**Thoughts** 
  - Built a payment form
  - Tested checkboxes, radio buttons, submit, reset, anonymous buttons, etc...
  
**Link(s)**
https://github.com/johncoenen/HTML/tree/master/payment-form
https://github.com/johncoenen/HTML/tree/master/form-fields

## Monday, January 8, 2018

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

## Wednesday, January 10, 2018

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

## Thursday, January 11, 2018

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

## Saturday, January 13, 2018

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

## Monday, January 15, 2018

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

## Tuesday, January 16, 2018

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

## Wednesday, January 31, 2018

**Today's Progress**:
- Continued CSS Grid Course work 
- auto-fit and auto-fill
- minmax() and media queries
- grid-template-areas
- naming areas in CSS grid

**Link(s)**
https://github.com/johncoenen/CSS-Grid-with-Wes-Bos-Coursework

## Saturday/Sunday, February 3/4, 2018

**Weekend Progress**:
- Visited https://www.codecademy.com and completed 25% each of Python and SQL tutorials
- Continued CSS Grid course
  - naming lines 
  - auto-flow-dense for Block Fitting
  - alignment and centering - similar to Flexbox
  - reordering items
  - 1st of the larger scoped projects - Nested Grid with Album Layout
  
**Link(s)**
https://github.com/johncoenen/CSS-Grid-with-Wes-Bos-Coursework

## Tuesday, February 6, 2018

**Today's Progress**: 
  - Worked through 1 - 9 of bash shell scripting tutorial
  
**Thoughts** 
  - Not something i've ever delved into, but found quite educational and enjoyable
  - side note: finally figured out how to change the colors in vim.rc
  
**Link(s)**
https://www.shellscript.sh/index.html

## Wednesday, February 7, 2018

**Today's Progress**: 
  - Refresher on SQL databases using Codecademy tutorial
  
**Thoughts** 
  - Haven't created/used a ton of databases, so this is just a little brush up.

**Link(s)**
  - https://www.codecademy.com/learn
  

## Thursday, February 8, 2018

**Today's Progress**: 
  - Decided to look into Bootstrap
  - Began W3 Schools tutorials
  
  **Thoughts** 
  - Another area that I am not well versed in(use CSS3 instead for most of what I covered today, but there is a lot of other useful stuff here that will eventually be covered).
  - Not as demanding as I thought, that being said I only just touched the basics today.

**Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp
  - https://github.com/johncoenen/Bootstrap-w3schools

## Sat./Sun., February 10/11, 2018

**Today's Progress**: 
 - Bootstrap continued
    - Jumbotron
    - Buttons
  - Tooks some notes on Networking
  - Looked at little more bash shell scripting(loops specifically)
  - Need to learn more about grep as well  

**Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp
  - https://github.com/johncoenen/Bootstrap-w3schools


## Tuesday, February 13, 2018

**Today's Progress**: 
  -Bootstrap continued
    - Glyphicons
    - Badges/Labels  

**Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp
  - https://github.com/johncoenen/Bootstrap-w3schools

## Thursday, February 15, 2018

**Today's Progress**: 
  -Bootstrap continued
    - Progress Bars
    - Pagination
    - Pager

**Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp
  - https://github.com/johncoenen/Bootstrap-w3schools
  
## Sat/Sun, February 17/18, 2018

**Today's Progress**: 
  -Bootstrap continued
    - List Group
    - Panels
    - Dropdowns
  
  - Purchased a discounted CLI course from Remy Sharp
  * Covered the first 10 introductory videos
  * Going through the basics of using the command line on MAC | Windows | Linux
  * Got to use the bash interface on Windows a little more
  * Most of this was refresh material, but always good to hear/see how a pro does it
  
**Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp
  - https://github.com/johncoenen/Bootstrap-w3schools
  - https://remysharp.com/2017/03/15/terminal-training

**Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp
  - https://github.com/johncoenen/Bootstrap-w3schools
  
## Wednesday February 21, 2018
**Today's Progress**:  
  - Bootstrap continued
    - Collapse
    - Tabs and Pills
    - Navigation Menus
  
  **Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp
  - https://github.com/johncoenen/Bootstrap-w3schools

## Friday, February 23, 2018
**Today's Progress**:  
  - Bootstrap continued
    - Forms
    - Slow moving, lately, but getting a hang of things

  **Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp
  - https://github.com/johncoenen/Bootstrap-w3schools

## Sunday/Monday February 25/26, 2018
**Today's Progress**:  
  - Bootstrap continued
    - Inputs 
    - Input Sizing
    - Media Objects
    
  **Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp  
  - https://github.com/johncoenen/Bootstrap-w3schools
  
  ## Tuesday February 27, 2018
**Today's Progress**:  
  - Bootstrap continued
    - Carousel
    - Modal
    - Popover    
    
  **Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp  
  - https://github.com/johncoenen/Bootstrap-w3schools

  ## Monday March 5, 2018
**Today's Progress**:
  - Worked on this over several sessions last week
  - Bootstrap (main area) Finished!
    * Scrollspy
      * Horizontal Nav Scrollspy
      * Pills Sidebar Nav Scrollspy
    * Affix
      * Sticky Horizontal Navigation
      * Sticky Vertical Navbar
    * Filters
    
  **Link(s)**
  - https://www.w3schools.com/bootstrap/default.asp  
  - https://github.com/johncoenen/Bootstrap-w3schools

## Wednesday April 11, 2018
**Today's Progress**:
- Away for a bit, but now I'm back better than ever.
- Haven't strayed from the code world, just reading a lot and not working on many projects
- Beginning an online React course this week
- Today I will be working on some of the pre-course material, specifically understanding the "this" keyword in Javascript

**Link**
- https://tylermcginnis.com/this-keyword-call-apply-bind-javascript/

## Thursday April 12, 2018
**Today's Progress**:
- Watched first part of day one video and coded along
- Used React CDN links
- created simple first portion of first React app example

**Links**
Shout out to Tyler McGinnis for the free course!
- https://tylermcginnis.com/
- https://github.com/johncoenen/React_Bootcamp.git
- CDN Links: https://reactjs.org/docs/cdn-links.html#___gatsby
- React Devtools: https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en

## Friday April 13, 2018
**Today's Progress**:
- Finished second part of day1 video
- Used create element API then moved on to components
- Learned difference btwn. elements and components
- Introduced to JSX
- Used components to render UI elements using JSX

**Links**
- https://github.com/johncoenen/React_Bootcamp.git
