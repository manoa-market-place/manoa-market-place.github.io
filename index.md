# Manoa Marketplace
_An online marketplace of all things you can buy/sell for the 'Bows!_



## Table of contents
* [Overview](#overview)
* [Deployment](#deployment)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)
* [Contact Us](#contact-us)

## Overview
Manoa Marketplace is a web application for UHM students to facilitate buying and selling of student-related goods and services.

### Approach
* Buyers and sellers must be UH students, faculty, or staff
* There is no anonymity: buyers and sellers connect through their UH credentials
* Transactions are expected to occur on-campus. If a seller wants to meet off-campus, that can be a red-flag
* Because buyers and sellers are from UHM, the goods and services will be relevant to UH students

### Implementation
Manoa Marketplace is designed with the following technologies:
* [Meteor](https://www.meteor.com/) for Javascript-based implementation of client and server code
* [Bootstrap 5 React](https://react-bootstrap.github.io/) for user interface
* [Uniforms](https://uniforms.tools/) for form development


## Deployment
See the [Manoa Marketplace]() in deployment through [Digital Ocean](https://www.digitalocean.com/)


## User Guide
This section provides a walkthrough of the Manoa Marketplace user interface and its capabilities.



## Community Feedback
We are eager to know how you liked the Manoa Marketplace! After experiencing with the application, please take a couple of minutes to fill out the [Manoa Marketplace Feedback Form](https://forms.gle/4wUn5QGKwvkbddfY6). It will greatly help us understand how our system is, improve 
existing features or implement new ones. Mahalo!


## Developer Guide
This section provides information of interest to Meteor developers wishing to use this application for their own development tasks.

### Installation
1. [install Meteor](https://www.meteor.com/install)
2. Visit the [Manoa Marketplace GitHub page](https://github.com/manoa-market-place/manoa-market-place), and click the "Use this template" button to create your own repository with initialized with a copy of this application. Alternatively, you 
   can download the source code as a zip file or make a fork of the repo. However you do it, download a copy of the repo to your local computer.
3. cd into the manoa-market-place/app directory and install libraries with:
   4. ```
      $ meteor npm install
      ```
4. Run the system with:
   5. ```
      $ meteor npm run start
      ```
5. If all goes well, you can view your application at [http://localhost:3000](http://localhost:3000)
6. You can login using the credentials in [settings.development.json](), or else register a new account.

### ESLint
YOu can verify that the code obeys our coding standards by running ESLint over the code in the imports/ directory with:
```
$ meteor npm run lint
```


## Development History

The development process for Manoa Marketplace conformed to [Issue Driven Project Management (IDPM)](https://courses.ics.hawaii.edu/ics314f23/morea/project-management/reading-guidelines-idpm.html) agile software process. Bottom line up front (BLUF):
* Process was managed using milestones which provide "deliverables" every 7-14 days.
* Within each milestone contains a series of tasks as GitHub Issues taking ideally 2~3 days to accomplish
* The work performed on each issue is in its own branch named "issue-XX", where XX is the issue number, and merged back into the main branch after its completion
* The status of each issue (todo, in progress, complete) under a milestone is managed using the GitHub Project Board

The following sections document the development history of the Manoa Marketplace.

### Milestone 1: Mockup Development
The goal of Milestone 1 (M1) was to set up the team, create initial issues, and deploy the initial application system to Digital Ocean with a landing page and at least four other mockup pages. 

M1 was managed using [Manoa Marketplace GitHub Project Board M1](https://github.com/orgs/manoa-market-place/projects/4):

### Milestone 2: Full Development
The goal of Milestone 2 (M2) was to continue manage the project and implement the core functionalities of the application.

M2 was managed using [Manoa Marketplace GitHub Project Board M2](https://github.com/orgs/manoa-market-place/projects/2):

### Milestone 3: Final Touches
The goal of Milestone 3 (M3) was to finish the project, acquire community feedback and implement acceptance testing.

M3 was managed using [Manoa Marketplace GitHub Project Board M3](https://github.com/orgs/manoa-market-place/projects/3):

### Beyond the basics
The follow contains yet-to-be-implemented ideas for more advanced features to the Manoa Marketplace:
* A rating system for buyers and sellers
* Map-based interface to indicate where goods are

### Links
* The [Manoa Marketplace GitHub organization](https://github.com/manoa-market-place)
  * [Home Page Repository](https://github.com/manoa-market-place/manoa-market-place.github.io)
  * [Project Template Repository](https://github.com/manoa-market-place/manoa-market-place)
* The Devs' [Team Contract]()





## Contact Us
Manoa Marketplace is designed, implemented, and maintained by the following developers:

* [Andrew Lin](https://andrewlin808.github.io/)
* [Baishen Wang]()
* [Bing Ying Li]()
* [Carlton Hung]()
* [Yujie He]()







<!--
BowFolios is an example web application that provides pages to view and (in some cases) modify profiles, projects, and interests. It illustrates various technologies useful to ICS software engineering students, including:

* [Meteor](https://www.meteor.com/) for Javascript-based implementation of client and server code.
* [React](https://reactjs.org/) for component-based UI implementation and routing.
* [React Bootstrap](https://react-bootstrap.github.io/) CSS Framework for UI design.
* [Uniforms](https://uniforms.tools/) for React and Semantic UI-based form design and display.

It also provides code that implements a variety of useful design concepts, including:

* Three primary collections (Profiles, Projects, Interests) as well as three "join" Collections (ProfilesInterests, ProfilesProjects, and ProjectsInterests) that implement many-to-many relationships between them.
* Top-level index pages (Profiles, Interests, and Projects) that show how to manipulate these six collections in various ways.
* Initialization code to define default Profiles, Interests, and Projects and relations between them.
* A simple Filter page to illustrate how to perform simple queries on the database and display the results.
* Use of Meteor Methods to illustrate how to simplify implementation of multiple collection updates.
* Use of indexes to enforce uniqueness of certain fields in the collections, enabling them to serve as primary keys.
* Authentication using the built-in Meteor accounts package along with Sign Up and Sign In pages.
* Authorization examples: certain pages are public (Profiles, Projects, Interests), while other pages require login (AddProject, Filter).
* Use of Meteor Assets to initialize the database (helpful when initialization exceeds settings file size limits).



### Landing Page

The landing page is presented to users when they visit the top-level URL to the site.

![](images/landing-page.png)

### Index pages (Projects, Profiles, Interests)

Bowfolios provides three public pages that present the contents of the database organized in various ways.

The Profiles page shows all the current defined profiles and their associated Projects and Interests:

![](images/profiles-page.png)

The Projects page shows all the currently defined Projects and their associated Profiles and Interests:

![](images/projects-page.png)

Finally, the Interests page shows all the currently defined Interests, and their associated Profiles and Projects:

![](images/interests-page.png)


### Sign in and sign up

Click on the "Login" button in the upper right corner of the navbar, then select "Sign in" to go to the following page and login. You must have been previously registered with the system to use this option:

![](images/signin-page.png)

Alternatively, you can select "Sign up" to go to the following page and register as a new user:

![](images/signup-page.png)

### Home page

After logging in, you are taken to the home page, which presents a form where you can complete and/or update your personal profile:

![](images/home-page.png)

### Add Project page

Once you are logged in, you can define new projects with the Add Project page:

![](images/add-project-page.png)


### Filter page

The Filter page provides the ability to query the database and display the results in the page. In this case, the query displays all of the Profiles that match one or more of the specified Interest(s).

![](images/filter-page.png)

## Community Feedback

We are interested in your experience using Bowfolio!  If you would like, please take a couple of minutes to fill out the [Bowfolios Feedback Form](https://forms.gle/hBHdccQEbm4YNfPd6). It contains only five short questions and will help us understand how to improve the system.

## Developer Guide

This section provides information of interest to Meteor developers wishing to use this code base as a basis for their own development tasks.

### Installation

First, [install Meteor](https://www.meteor.com/install).

Second, visit the [Bowfolios application github page](https://github.com/bowfolios/bowfolios), and click the "Use this template" button to create your own repository initialized with a copy of this application. Alternatively, you can download the sources as a zip file or make a fork of the repo.  However you do it, download a copy of the repo to your local computer.

Third, cd into the bowfolios/app directory and install libraries with:

```
$ meteor npm install
```

Fourth, run the system with:

```
$ meteor npm run start
```

If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000).

### Application Design

Bowfolios is based upon [meteor-application-template-react](https://ics-software-engineering.github.io/meteor-application-template-react/) and [meteor-example-form-react](https://ics-software-engineering.github.io/meteor-example-form-react/). Please use the videos and documentation at those sites to better acquaint yourself with the basic application design and form processing in Bowfolios.

### Data model

As noted above, the Bowfolios data model consists of three "primary" collections (Projects, Profiles, and Interests), as well as three "join" Collections (ProfilesProjects, ProfilesInterests, and ProjectsInterests).  To understand this design choice, consider the situation where you want to specify the projects associated with a Profile.

Design choice #1: Provide a field in Profile collection called "Projects", and fill it with an array of project names. This choice works great when you want to display a Profile and indicate the Projects it's associated with.  But what if you want to go the other direction: display a Project and all of the Profiles associated with it?  Then you have to do a sequential search through all of the Profiles, then do a sequential search through that array field looking for a match.  That's computationally expensive and also just silly.

Design choice #2:  Provide a "join" collection where each document contains two fields: Profile name and Project name. Each entry indicates that there is a relationship between those two entities. Now, to find all the Projects associated with a Profile, just search this collection for all the documents that match the Profile, then extract the Project field. Going the other way is just as easy: to find all the Profiles associated with a Project, just search the collection for all documents matching the Project, then extract the Profile field.

Bowfolios implements Design choice #2 to provide pair-wise relations between all three of its primary collections:

![](images/data-model.png)

The fields in boldface (Email for Profiles, and Name for Projects and Interests) indicate that those fields must have unique values so that they can be used as a primary key for that collection. This constraint is enforced in the schema definition associated with that collection.


## Initialization

The [config](https://github.com/bowfolios/bowfolios/tree/main/config) directory is intended to hold settings files.  The repository contains one file: [config/settings.development.json](https://github.com/bowfolios/bowfolios/blob/main/config/settings.development.json).

This file contains default definitions for Profiles, Projects, and Interests and the relationships between them. Consult the walkthrough video for more details.

The settings.development.json file contains a field called "loadAssetsFile". It is set to false, but if you change it to true, then the data in the file app/private/data.json will also be loaded.  The code to do this illustrates how to initialize a system when the initial data exceeds the size limitations for the settings file.


### Quality Assurance

#### ESLint

BowFolios includes a [.eslintrc](https://github.com/bowfolios/bowfolios/blob/main/app/.eslintrc) file to define the coding style adhered to in this application. You can invoke ESLint from the command line as follows:

```
meteor npm run lint
```

Here is sample output indicating that no ESLint errors were detected:

```
$ meteor npm run lint

> bowfolios@ lint /Users/philipjohnson/github/bowfolios/bowfolios/app
> eslint --quiet --ext .jsx --ext .js ./imports ./tests

$
```

ESLint should run without generating any errors.

It's significantly easier to do development with ESLint integrated directly into your IDE (such as IntelliJ).

#### End to End Testing

BowFolios uses [TestCafe](https://devexpress.github.io/testcafe/) to provide automated end-to-end testing.

The BowFolios end-to-end test code employs the page object model design pattern.  In the [bowfolios tests/ directory](https://github.com/bowfolios/bowfolios/tree/main/app/tests), the file [tests.testcafe.js](https://github.com/bowfolios/bowfolios/blob/main/app/tests/tests.testcafe.js) contains the TestCafe test definitions. The remaining files in the directory contain "page object models" for the various pages in the system (i.e. Home, Landing, Interests, etc.) as well as one component (navbar). This organization makes the test code shorter, easier to understand, and easier to debug.

To run the end-to-end tests in development mode, you must first start up a BowFolios instance by invoking `meteor npm run start` in one console window.

Then, in another console window, start up the end-to-end tests with:

```
meteor npm run testcafe
```

You will see browser windows appear and disappear as the tests run.  If the tests finish successfully, you should see the following in your second console window:

```
$ meteor npm run testcafe

> bowfolios@ testcafe /Users/philipjohnson/github/bowfolios/bowfolios/app
> testcafe chrome tests/*.testcafe.js

 Running tests in:
 - Chrome 86.0.4240.111 / macOS 10.15.7

 Bowfolios localhost test with default db
 ✓ Test that landing page shows up
 ✓ Test that signin and signout work
 ✓ Test that signup page, then logout works
 ✓ Test that profiles page displays
 ✓ Test that interests page displays
 ✓ Test that projects page displays
 ✓ Test that home page display and profile modification works
 ✓ Test that addProject page works
 ✓ Test that filter page works


 9 passed (40s)

 $
```

You can also run the testcafe tests in "continuous integration mode".  This mode is appropriate when you want to run the tests using a continuous integration service like Jenkins, Semaphore, CircleCI, etc.  In this case, it is problematic to already have the server running in a separate console, and you cannot have the browser window appear and disappear.

To run the testcafe tests in continuous integration mode, first ensure that BowFolios is not running in any console.

Then, invoke `meteor npm run testcafe-ci`.  You will not see any windows appear.  When the tests finish, the console should look like this:

```
$ meteor npm run testcafe-ci

> bowfolios@ testcafe-ci /Users/philipjohnson/github/bowfolios/bowfolios/app
> testcafe chrome:headless tests/*.testcafe.js -q --app "meteor npm run start"

 Running tests in:
 - Chrome 86.0.4240.111 / macOS 10.15.7

 Bowfolios localhost test with default db
 ✓ Test that landing page shows up (unstable)
 ✓ Test that signin and signout work
 ✓ Test that signup page, then logout works
 ✓ Test that profiles page displays
 ✓ Test that interests page displays
 ✓ Test that projects page displays
 ✓ Test that home page display and profile modification works
 ✓ Test that addProject page works
 ✓ Test that filter page works


 9 passed (56s)

$
```

All the tests pass, but the first test is marked as "unstable". At the time of writing, TestCafe fails the first time it tries to run a test in this mode, but subsequent attempts run normally. To prevent the test run from failing due to this problem with TestCafe, we enable [testcafe quarantine mode](https://devexpress.github.io/testcafe/documentation/guides/basic-guides/run-tests.html#quarantine-mode).

The only impact of quarantine mode should be that the first test is marked as "unstable".

## From mockup to production

Bowfolios is meant to illustrate the use of Meteor for developing an initial proof-of-concept prototype.  For a production application, several additional security-related changes must be implemented:

* Use of email-based password specification for users, and/or use of an alternative authentication mechanism.
* Use of https so that passwords are sent in encrypted format.
* Removal of the insecure package, and the addition of Meteor Methods to replace client-side DB updates.

(Note that these changes do not need to be implemented for ICS 314, although they are relatively straightforward to accomplish.)

## Continuous Integration

![ci-badge](https://github.com/bowfolios/bowfolios/workflows/ci-bowfolios/badge.svg)

BowFolios uses [GitHub Actions](https://docs.github.com/en/free-pro-team@latest/actions) to automatically run ESLint and TestCafe each time a commit is made to the default branch.  You can see the results of all recent "workflows" at [https://github.com/bowfolios/bowfolios/actions](https://github.com/bowfolios/bowfolios/actions).

The workflow definition file is quite simple and is located at
[.github/workflows/ci.yml](https://github.com/bowfolios/bowfolios/blob/main/.github/workflows/ci.yml).

## Development History

The development process for BowFolios conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f19/modules/project-management/) practices. In a nutshell:

* Development consists of a sequence of Milestones.
* Each Milestone is specified as a set of tasks.
* Each task is described using a GitHub Issue, and is assigned to a single developer to complete.
* Tasks should typically consist of work that can be completed in 2-4 days.
* The work for each task is accomplished with a git branch named "issue-XX", where XX is replaced by the issue number.
* When a task is complete, its corresponding issue is closed and its corresponding git branch is merged into master.
* The state (todo, in progress, complete) of each task for a milestone is managed using a GitHub Project Board.

The following sections document the development history of BowFolios.

### Milestone 1: Mockup development

The goal of Milestone 1 was to create a set of HTML pages providing a mockup of the pages in the system.

Milestone 1 was managed using [BowFolio GitHub Project Board M1](https://github.com/bowfolios/bowfolios/projects/1):

![](images/project-board-1.png)

### Milestone 2: Data model development

The goal of Milestone 2 was to implement the data model: the underlying set of Mongo Collections and the operations upon them that would support the BowFolio application.

Milestone 2 was managed using [BowFolio GitHub Project Board M2](https://github.com/bowfolios/bowfolios/projects/2):

![](images/project-board-2.png)

## Milestone 3: Final touches

The goal of Milestone 3 was to clean up the code base and fix minor UI issues.

Milestone 3 was managed using [BowFolio GitHub Project Board M3](https://github.com/bowfolios/bowfolios/projects/3):

![](images/project-board-3.png)

As of the time of writing, this screenshot shows that there is an ongoing task (i.e. this writing).
-->

