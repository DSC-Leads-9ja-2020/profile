# Profile
Contains code for the website where we can manage our profiles and where everyone can search and see each other

## About

### Background
We are all different and all have different things identifying us. Keeping in mind of each persons peculiarities (name, social media profiles, school/location, skills, ...) could be difficult. We used Google Slides and Google Sheets to save our names, social media links and schools. Everyone had access to them and will come in and put their profile. However, we could not prevent some fatal mistakes, such as, someone wrongly editing another person's details or someone deleting the all the data. These errors eventually occured and we look out to make member profile lookup and maintenance easy. Besides, a spreadsheet's user interface is not suitable for such; for example, uploading profile pictures is incovenient. 

### Problem Statement
We want an easy way to quickly search for members using their names, schools, location(state) or skills. We want to have all details about members, listed in such a way to ease follow up and interaction. We also want each member to be the only person in charge of their data/details.

### Proposed Solution
What if we had a platform whose main objective is store and show members profiles, make it  easy to find members based on the various filters, and give members the opportunity to sign in and create, update or delete their profile details. We will build it as a web app with plain HTML, CSS and vanilla (plain) JavaScript, without the aid of any frameworks/libraries. We will use Firebase for the app's backend. 

### Target Audience
Members (in this case, us DSC Leads)

### User Stories:
As a member I can ...
* sign in with Google to access the platform
* verify my phone number on first sign in
* update my name and phone number
* add/update/delete the following
  * my profile picture
  * more emails and phone numbers belonging to me
  * town(s) and state(s) where I live/school/can be found
  * social media, portfolio or other profile links
  * the school I am a DSC lead for my DSC Chapter's social media and website links
* view every other member (picture and name) on the landing page after signing in 
* expand/open a member to view their complete their profile
* click on the links on a members profile to follow through to their websites
* click on call button to get their number in my dial pad or whatsapp button to message them directly
* view members' DSC Chapter logo and name, and click through links pertaining to their DSC 
* can search for members based on attributes and can set which attribute to use
* view my profile the way others view it
* can sign out

Features (Pages):
All pages will contain a header with DSC logo and our title in it.

1. Landing/Sign In Page (Sign In with Google only) and Phone Verify (Shown at first Sign In after sign in with Google). It will have a header with DSC Logo and we will use the FirebaseUI (https://github.com/firebase/firebaseui-web) library for sign in and phone verify. So less coding and less design needed here. Only signed in users should access other parts of the platform.

2. Settings Page. A page that contains forms and buttons to manage or delete all details mentioned in the above user stories.

3. Home Page. Aside header, it will contain the following:
  a. a top navbar with just two buttons, that will persist across other pages, when signed in. One button should link to the settings page (this navbar should also be present in the settings page), while the other button will be to sign out.
  b. search bar to search members generally. And a way to search members based on peculiar attributes (maybe based on only their location, their skills, school...) 
  c. profile cards of members' pictures, names and more button/link to view their full profile

4. Profile Details page where one can view and interact with all the details of a particular member at a particular time, (the signed-in member should see their own profile details page too).


## Angular 

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 11.0.5.

### Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

### Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

### Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

### Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

### Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

### Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
