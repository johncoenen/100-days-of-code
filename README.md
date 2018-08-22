## Personal Log 

## Monday, January 1, 2018

**Today's Progress**: 
  Created a basic ASP.NET MVC app
  
**Thoughts** 
  - Nice to revisit Visual Studio after some time away
  - Learned the basic fundamentals that go into creating a MVC application
  - Understand how Views are created and manipulated within the ASP.NET stack
  
**Link(s)**
- https://github.com/johncoenen/ASP.NET-MVC---Basic-Template

## Tuesday, January 2, 2018

**Today's Progress**: 
  Created a basic responsive web app with HTML5 and CSS Media Queries(from demo)
  
**Thoughts** 
  - Quick and dirty project
  - Using HTML5 semantics and media queries
  - First time really using Emmet shorthand in VSCode!
  - TODO: fix issues with font awesome icons, change styling/markup to be more accessible
  
**Link(s)**
- https://github.com/johncoenen/QuickApps/tree/master/ResponsiveApp_HTML5_CSS

## Wednesday, January 3, 2018

**Today's Progress**: 
  Begin looking at jQuery UI, starting with draggable DOM elements
  
**Thoughts** 
  - Easy to user interface
  - Less javascript than expected
  - First time really using jQuery  
  
**Link(s)**
- https://github.com/johncoenen/jQuery

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
- https://www.digitalocean.com/community/tutorial_series/understanding-the-dom-document-object-model

## Friday, January 5, 2018

**Today's Progress**: 
  Began HTML Forms tutorial, with emphasis on how screen readers interpret forms
  
**Thoughts** 
  - Looked at how screen readers order the elements of a form
  - Learned best practices for required field form elements
  
**Link(s)**
- https://github.com/johncoenen/HTML/tree/master/forms-screen_reader

## Sat/Sun, January 6/7, 2018

**Today's Progress**: 
  Continue HTML forms tutorials looking at payment form and formfield input widgets

**Thoughts** 
  - Built a payment form
  - Tested checkboxes, radio buttons, submit, reset, anonymous buttons, etc...
  
**Link(s)**
- https://github.com/johncoenen/HTML/tree/master/payment-form
- https://github.com/johncoenen/HTML/tree/master/form-fields

## Monday, January 8, 2018

**Today's Progress**: 
  Build ASP.NET Core Angular application from tutorial
  
**Thoughts** 
  - It's a miracle this works at all, but I will call this a win
  - The tutorial was well written and I only had a few workarounds and bugs to deal with
  - First time getting an Angular app running with Visual Studio 2017
  - Will be continuing this tutorial tomorrow and adding enhancments  
  
**Link(s)**
- Tutorial: 
    - https://medium.com/@levifuller/building-an-angular-application-with-asp-net-core-in-visual-studio-2017-visualized-f4b163830eaa     
- Demo:    
    - https://github.com/johncoenen/ASP.NET-Angular-Starter

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
- Tutorial: 
    - https://medium.com/@levifuller/building-an-angular-application-with-asp-net-core-in-visual-studio-2017-visualized-f4b163830eaa
 
- Demo: 
    - https://github.com/johncoenen/ASP.NET-Angular-Starter 

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
- tutorial: 
    - https://angular.io/tutorial (Tour of Heroes)
- demo: 
    - https://github.com/johncoenen/Angular-Tour-Of-Heroes

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

**Link**
- https://github.com/johncoenen/Angular-Tour-Of-Heroes 

## Tuesday, January 16, 2018

**Today's Progress**:
  - Started a project currated by Sarah Drasner called Creating a Vue.js Serverless Checkout Form: Setup and Testing. 
  - Set up Azure and Stripe accounts
  - Configured basic serverless funciton application using Azure
  - set up application architecture using node and npm

**Thoughts**
  - Straight forward and easy to follow tutorial with code examples made getting started a breeze

**Link**
- https://css-tricks.com/creating-vue-js-serverless-checkout-part-one/

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
- Link to free course:  
    - https://cssgrid.io/
- Link to my work: 
    -https://github.com/johncoenen/CSS-Grid-with-Wes-Bos-Coursework

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
- https://github.com/johncoenen/Angular-Tour-Of-Heroes

## Wednesday, January 31, 2018

**Today's Progress**:
- Continued CSS Grid Course work 
- auto-fit and auto-fill
- minmax() and media queries
- grid-template-areas
- naming areas in CSS grid

**Link(s)**
- https://github.com/johncoenen/CSS-Grid-with-Wes-Bos-Coursework

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

## Monday April 16, 2018
**Today's Progress**:
- Took notes on React Bootcamp Day 2 pre-reading (React Elements vs React Components)
- Watched add coded along with first portion of day 2 video
- Built simple friends list apps
  - First using a Function Component 
  - Second using a Class based Component
  
**Links**
- https://www.youtube.com/watch?v=NHfRLQuHjsU&t=1788s
- https://github.com/johncoenen/React_Bootcamp.git

## Tuesday April 17, 2018
**Today's Progress**:
- continue day two React Bootcamp video
- code along with Gist 4(friendsList_3.html) and Gist 5(friendsList_4.html)
- Remember this.setState will update the state then update the UI
- React has a currentState method
    - We create a function to remove a name from the friends list
    - pass this function to this.setState using the currentState method
    - this function returns and object that will update the state and merge with currentState and change the UI
    - Add delete button to App, passed prop to friends list in JSX area, add onClick event here as well
    - use this keyword on handle.RemoveFriends in the return method
    - used .bind(this) to specify where the this keyword is referencing so that the UI can be updated

**Links**
https://github.com/johncoenen/React_Bootcamp.git
    
## Wednesday April 18, 2018
**Today's Progress**:
- finish Gist 6 of day two React Bootcamp
- code along with Gist 6(friendsList_5.html)
- Create the Add Friend Area
- We get the user input from what is written in the form area and a submit button
- Add state to the live componet then update the state when user pushes submit
- Then we update the property in the JSX, needed to add onChange event to update the input
- Finish the AddFriend function using this.setState passing it a function(=>) 
- Return the new state and merge with previous state then concat new item onto that state
- Add the new name to the list
- Delete the name from the input box

**Links**
https://github.com/johncoenen/React_Bootcamp.git

## Thursday April 19, 2018
**Today's Progress**:
- finish Gist 7 of day two React Bootcamp
- code along with Gist 7(friendsList_6.html)
- Added Active/Inactive friends areas and inputs 

**Links**
- https://github.com/johncoenen/React_Bootcamp.git

## Saturday/Sunday April 21-22, 2018
**Today's Progress**:
- No React this weekend, will continue this upcoming week
- Completed chapters 1 - 4 for CLI for Front End Developers by Remy Sharp
- Here is a list of the subject matter covered in these videos/chapters
  - Navigating directores
  - Navigation shortcuts
  - Running applications
  - Connecting programs using pipe(s)
  - Searching through files using grep, . find, etc.
  - String manipulation and Regular Expression (egrep)
  - Head, tail, and less for outputing data
  - Sort and Uniq for filtering data 
  - Deleting all things
  - Permissions with sudo, chmod, and chown
  - Killing processes
  - Health checking with df, du, top, and htop
  
  **Links**
  - https://remysharp.com/2017/03/15/terminal-training
  
  ## Monday April 23, 2018
  ** Today's Progress**:
  - Got a bit ahead of myself by accident and did the React-Bootcamp day 4 pre-reading
  - Coded along with the video covering React Router v4
  - The example is not working, but I will have to get this going using Create React App
  - As of now it is just a messy .js file
  - Important takaways:
    - v4 uses Dynamic Routing
    - everything is a component
    - use the ({match}) property rather than hard coding routes so that if changes get made they don't need to be changed individually
    - use ({match}) with template strings like $(match.url) to create routes
    
    **Links**
    - https://tylermcginnis.com/react-router-philosophy-introduction/
  
  ## Tuesday April 24, 2018
  **Today's Progress**:
  - Day 3 Tyler McGinnis React Bootcamp part 1 of video
  - Code along for Gists 1 - 3
  - Takeaways:
    - Learned about the course a React component takes during it's lifecycle
    - Constructor->Rende->componentDidMount->componentDidUpdate->componentWillUnmount
    - componentDidMount is the part of the life cycle where AJAX requests are made to APIs or databases to retrieve data
  
  **Links**:
  - https://github.com/jdmedlock/mcginnisreact/blob/master/Day3/gist31.html
  - https://github.com/jdmedlock/mcginnisreact/blob/master/Day3/gist32.html
  - https://github.com/jdmedlock/mcginnisreact/blob/master/Day3/gist33.html
  - https://www.youtube.com/watch?v=Xa3DGGP4mLM&t=2829s
  - https://github.com/johncoenen/React_Bootcamp.git
  
   ## Wednesday April 25, 2018
  **Today's Progress**:
  - Day 3 Tyler McGinnis React Bootcamp part 2 of video
  - Code along for Gists 4,5,6
  - Takeaways:
      - Add Loading UI to the app
      - Cleanup simple Loading UI and add simple animation to it
      - Looked at componentDidMount, componentDidUpdate, and componentWillUpdate in real world examples
      
  **Links**:
  - https://www.youtube.com/watch?v=Xa3DGGP4mLM&t=2829s 
  - https://github.com/johncoenen/React_Bootcamp.git 
  - https://gist.github.com/tylermcginnis/33f883b4cfa7b8a4e449414b96171805
  - https://gist.github.com/tylermcginnis/e3822fb9a73ecec62c814e4a14c3229e
  - https://gist.github.com/tylermcginnis/29f885fdb5d9d5206e6fedc9168134aa
  
## Thursday April 26, 2018
**Todays Progress**:
- Watched chapter 5 (1-7) videos for Remy Sharp's CLI for Frontend Developers crash course
- Learned about some popular shells and how to customize them to your liking, fish shell z(zed)shell
- Worked with Aliases to create shortcuts for commands, as well as to run fuunctions

**Links**
- http://ohmyz.sh/ - popular z shell framework
- https://fishshell.com/
- https://github.com/remy/dotfiles - lots of aliases and functions to snatch

## Friday April 27,2018
**Today's Progress**:
- Quick CSS Grid: Spanning and Placing Cardio session this morning
- Create quick grid example also on codepen

**Link**:
- https://codepen.io/ofoshoJC/pen/ZoWByZ
- https://codepen.io/ofoshoJC/full/JvbwGE

## Saturday April 28, 2018
**Today's Progress**:
- Little UI lesson from Medium article on creating Flexbox UI
- Need to make this responsive, maybe go back and finish the other suggestios(Facebook, Github, Medium)
- Love the magic that happens using margin: auto inside the twitter__bird styles
- TODO: try this with Grid / Grid + Flexbox fallbacks

**Link**:
- https://developer.mozilla.org/en-US/docs/Web/HTML/Element/main
- https://codepen.io/ofoshoJC/pen/JvEXwx?editors=1100

## Sunday April 29, 2018
**Today's Progress**:
- Coded along with the video on Bootsrappy CSS Grid with CSS variables in Wes Bos's CSS Grid video course
- Used CSS variables to set span sizing of grid items using them as inline style elements
- Pseudo framework of how to create a Bootstrap like grid with raw css(grid and variables together)

**Links**:
- https://cssgrid.io/?ref=prototyprio
- https://github.com/johncoenen/CSS-Grid-with-Wes-Bos-Coursework/tree/master/24%20-%20BootstrappyGridwithCSSVariables

## Friday, Saturday, Sunday May 4,5,6 2018
- Started a new repo for some example websites
- Goal: Portfolio/Proof of Concept Website pushing my personal brand
- Using Bootstrap 4 and Bootstrap Material Design
- Loosely working off a template from viewing source code for: https://mdbootstrap.com/previews/templates/portfolio/html/graphic-designer.html#
- Looking up stuff I don't know along the way and implementing what I like as I build the site by section
- Quick brush up on git some too at:
  - https://www.codecademy.com/learn/learn-git
**Links**
- https://github.com/johncoenen/Web-Site-Examples
- https://fezvrasta.github.io/bootstrap-material-design/

## Monday May 7, 2018
- continued working on portfolio demo site
- Not implementing the Jarallax library yet
- Tommorow = look at Jarallax tutorials
- not sold on parallax scrolling, may have to keep this demo parallax free

**Links**
-- https://github.com/johncoenen/Web-Site-Examples


## Monday May 14, 2018
- Picked up Atomic Design by Brad Frost
- Start looking at Pattern Lab

## Tuesday May 15, 2018
- Couldn't really get up and running with Pattern Lab node or php versions
- Kind of tricky install - had to find a compatable version of node
- At the end of the day I couldn't get either set up nailed down, will look at Pattern Lab 2 tommorow

## Wednesday May 16, 2018
- Installed the PHP version of Pattern Lab 2 on Ubuntu 16.04
- Seems to be working at the moment 
- Some take aways:
  - Need mustache installed in order to use the templating language
  - For PHP, Composer needs to be installed(locally or globally) for Pattern Lab to run
  - Pattern Lab comes with a built in server to run on
  - Need to learn mustache syntax to get started using pattern lab
  - Not quite sure how this works yet, my guess is that I need to mess with the JSON file to output data through the mustache file(s)
  
## Sunday May 20, 2018
- Not much coding this week, but lots of reading
- Did some design work over the weekend
- Created a svg illustration which was then converted to jpg format
- Used the illustration as a background image in Codpen and made it cover the entire screen responsively

## Saturday May 26, 2018
- Another uneventful week
- A lot of interview prep stuff this week in lieu of code
- I did manage to find some time to get in a little Codpen action. Was inspired by the Netflix series Mindhunter and how they introduce the setting using text: https://codepen.io/ofoshoJC/pen/yjmzWN
- The text-shadow effect overlaps on smaller devices, but it remains legible
- The text and image in the header are responsive, and the lorem... dummy text was added to see how it would look with a page layout


## Saturday June 3, 2018
- Not a lot of code this week
- Spent most of my time preparing for interviews
- Did get some time in today working on a new repo for all things forms
- This is a skill-set employers are looking for in frontend devs
- Starting with the good old standby, MDN Forms 
- Completed three sections dealing with form elements
- These are sometimes verbatim written from the tutorials, I would never use this material for a live project because, duh!, plagarism.
- This just helps me commit stuff to memory

**Today's progress:**
  - Basic Forms
  - Form Structure
  - Native Widgets

**Links**
  - https://github.com/johncoenen/Forms
  - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms 
  
## June 5/6, 2018
 - ...more MDN form stuff....
 - added Native Form Widget sectiom to repo
 - added Advanced Form Widget section to repo
 - Am going to skip the last (Other Widget) section for now and move on to more advanced form handling
 - took too long with this section doing every example, which sort of mirrors the Bootsrap W3 tutorials 

**Links**
  - https://github.com/johncoenen/Forms
  - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms
  
## June 8, 2018
 - ...more MDN form stuff....
 - Started refresher on HTTP protocol and how forms are sent

**Links**
  - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Sending_and_retrieving_form_data

## June 9, 2018
 - Decided to take a break from forms, moved on to using Github Pages
 - Changed my Terminator theme too!
 - Opened a repo for a portfolio style website
 - Spent the rest of the evening looking at responsive background images, for a landing page, using webp and jpg formats with media queries, in HTML

**Links**
  - https://github.com/johncoenen/johncoenen.github.io
  
  ## June 13/14 2018
 - back to form stuff
 - Added section on sending data along with how the GET & POST methods work
 - Reviewed differences btwn. sending in the browser(client side) versus sending data to the server(server side)
 - Began section on form validation

**Links**
  - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Sending_and_retrieving_form_data
  - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Form_validation
  - https://github.com/johncoenen/Forms/tree/master/Validation
  - https://github.com/johncoenen/Forms/tree/master/SendingData

  ## June 16/17 2018
 - back to MDN: Form Validation
 - Looked at different types of HTML form validation
   - Client side validation
   - Server side validation
   - constarints on inputs
   - required field
   - regex validation
   - constarining length
 - Validation with Javasctipt methods
 - create custom error messages using the constraint validation API
 
 **Links**
 - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Form_validation
 - https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5/Constraint_validation
 - https://github.com/johncoenen/Forms
 
 ## June 18, 2018
 - Started customizable form widgets section of MDN: Forms
 - Designed the types of state we would be using: active, open, value change
 - styled the widget to show when user has selected an item in the options list
 - TODO: tomorrow complete the javascript section and give the widget some life
 
 **Links**
 - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/How_to_build_custom_form_widgets
 - https://github.com/johncoenen/Forms/tree/master/CustomFormWidgets
 
 ## June 19, 2018
 - Short session today
 - Added some Javascript and CSS selectors to hide form elements as fallback if js is not working.
 - Most browsers fully support Javascript now, so this is not a huge issue
 - Ran into an error that wanted me to set mouse scroll events to "passive" 
 - TODO:  try running the script with only one widget option, and look into setting events as "passive"
 - TODO: finish up final portion of the custom form widgets section 
 
 **Links**
 - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/How_to_build_custom_form_widgets
 - https://github.com/johncoenen/Forms/tree/master/CustomFormWidgets
 
 # June 25, 2018
 - More with MDN Forms, today I added the second version of the form which will leverage the DOM API to do the work 
 - This form will use callbacks to initialize the elements
 - Added event handlers for:
    - selecting an option from the dropdown list
    - activate/deactivate the widget
    - turn on/off the active state of the widget 
    - open/close the list of options
    - highlight the selected option in the dropdown list
    
  **Links**
  - https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/How_to_build_custom_form_widgets
  - https://github.com/johncoenen/Forms/blob/master/widget_1.02.html

# June 26/27, 2018
- MDN Forms:
  - worked on handling the changing dropdown values from the option list
  - worked on binding custom widget with native widget
  - still have some work to do to get this correct, but much progress was made
  - on to v1.05 of this widget
  
**Links**
- https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/How_to_build_custom_form_widgets
- https://github.com/johncoenen/Forms/tree/master/CustomFormWidgets

# June 29/30
- MDN Forms:
  - finished working example of widget 
  - added ARIA accesibility for assitive technologies

**Links**
- https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/How_to_build_custom_form_widgetsF
- https://github.com/johncoenen/Forms/blob/master/CustomFormWidgets/widget1.06.html


# July 7/8 2018
- Note: add anything I may have missed btwn end of June and this date...Note2- wordpress build for portfolio
- Began working on some typesetting for the web
- Taking inspirartion from print and photo shop documents to create responisve web pages
- Created an "About" page template using HTML5
- Created a responsive layout using Flexbox, percentages, and rem units for fonts
- Using Google fonts for type

- TODO: 
  - complete lower portion of the page along with footer
  - possibly add media queries to avoid breaking on different devices, but so far it works alright

**Links**
- https://github.com/johncoenen/Web-Typography
- https://codepen.io/ofoshoJC/pen/XYvjZd?editors=1100

# July 12 2018
- worked on some prototyping using Figma
- Figma is cool, really intuitive and easy to jump into
- Started a webpage layout
- Need to learn more about how layers work in Figma in order to export something tangible

**Links**
- https://www.figma.com/file/OFl7SmRmpkhbvNOfmMXHLZn4/SPA-1

# July 17 2018
- just a little prototyping today...

**Links**
- https://www.figma.com/file/NnqSRcFYj6tnyBwr0Z92aoeL/Card-Layout

# July 21,22 2018
- more prototyping with figma
- this is an excellent tool for creating visual mock ups of logos, websites, forms, icon sets, style tiles, etc
- made a mock logo - https://www.figma.com/file/dL42spYGodJdoG3wPGWRB8lg/PipelineProductions
- made a font combination card - https://www.figma.com/file/cY66BctlOAPBgMtDCelECeiX/Oswald-and-EB-Garamond

# July 24 2018
- FIGMA!
- made a master component prototype that includes icons, font, and button styles.
- https://www.figma.com/file/ZAe7byBFcUO8PA3HNglzTxUf/Component-Ex.

# July 25 2018
- again with the Figma
- made a simple phone login form w/ button
- https://www.figma.com/file/UAzgJSW5DRb5zSmLL7djgXWW/LOGIN 

# July 26 2018
- you guessed it, more Figma
- made a media object with nested media objects prototype
- https://www.figma.com/file/0h0QWx8Ec9KnJJ2RZYKicEta/Media-Object

# July 28 2018
- began working on github page that will be used as my portfolio
- basic template w/ HTML & CSS complete
- https://github.com/johncoenen/johncoenen.github.io

# July 29 2018
- made some tweaks, took out CSS reset and used normalizer instead
- got the navigation, heading, and blockquote to where I want them
- https://github.com/johncoenen/johncoenen.github.io

# July 30 2018
- added additional media queries for when design breaks, rather than for devices, via advice from Smashing article by Rachel Andrew
- whole page is responsive, need to figure out how to repeat this throughout site
- TODO: complete footer section with icons, add actual images
- - https://github.com/johncoenen/johncoenen.github.io

# Vacation.....

# August 16-19 2018
- created a repo for CSS grid refresher 
- Using Grid By Example website as reference
- going through examples 
- getting better with Emmit for HTML and CSS

**Links**
* https://github.com/johncoenen/css-grid-refresh
* https://gridbyexample.com/

# August 21 2018
- quick grid by example addition to css refresher repo 
- added section that shows why clearing with floats isn't necessary when using grid, because content will stay within the assigned grid tracks
- began demo of a music app using css grid from a Medium article

**Links**
* https://github.com/johncoenen/css-grid-refresh
* https://gridbyexample.com/
* https://medium.com/flexbox-and-grids/how-to-efficiently-master-the-css-grid-in-a-jiffy-585d0c213577

# August 22 2018
* updated .json in Angular-Tour-Of-Heroes repo
