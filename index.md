## Table of contents

* [Overview](#overview)
* [Goal](#goal-of-the-application)
* [User Guide](#user-guide)
* [Developer Guide](#developer-guide)
* [Community Feedback](#community-feedback)
* [Development History](#development-history)
* [Contact Us](#contact-us)

## [Hi-Covid-Convo Site](https://cece-convo.xyz/)

## Overview
Welcome to HI-Covid-Convo! The goal of this project is simple. We're aiming to provide an easy-to-use chat-bot for those concerned with COVID-19. Whether it's directly answering user's questions, or redirecting them to useful resources, we hope to give all users peace of mind.
[To hi-covid-convo organization](https://github.com/hi-covid-convo)

## Goal of the Application
Over the next month, we plan to improve upon the applications functionality. By the end, our goal is to have a working chat-bot that will be able to answer COVID-related FAQs. Along with being able to parse user input and determine the best response/resource to provide, we also would like to include other resources on the site that will provide general information on COVID and how to remain safe during this pandemic. Because we want the site to remain anonymous, we plan to collect feedback statistics from users who use the chatbot. These statistics would include the most commonly asked questions, as well as how happy users are with the quality of the responses. These statistics would be available to an admin user once logged into the application.

# User Guide
### Our Current Progress..

## Landing Page
Users will first be taken to the landing page which will give an overview of the application. There is also a button to take them to Cece, the COVID chatbot. This page also discusses the goal for this application, and directs the user to go to the About page if they want to learn more

<img src = "./images/milestone1/landing.png">
You can view our landing page [here](https://cece-convo.xyz/#/).


## Cece the Chatbot
The button on the landing page will then take users to the Cece chatbot page. The page has a brief introduction to our chatbot Cece and some instructions on how to use it. On the right side of the screen is where the user will be able to enter in a question (as of now, the chatbot is still in progress and not fully complete).

<img src = "./images/milestone1/cece.png">
You can view our Cece Chatbot page [here](https://cece-convo.xyz/#/Cece).


## About Page
If the user wants to learn more about our application and its goal, they can visit the About page via the navigation bar. In this page we briefly go over what our goal is, and our purpose for creating this application.

<img src = "./images/milestone1/about.png">
You can view our About page [here](https://cece-convo.xyz/#/about).


## General COVID Info Page
The General knowledge page provides the user any general knowledge information about COVID-19. This includes topics like symptoms of the virus, how it is spread, and prevention and protection. This information was gathered from the [Centers for Disease Control and Prevention (CDC)](https://www.cdc.gov/coronavirus/2019-ncov/index.html). The General knowledge page is currently still in progress as well.

<img src = "./images/milestone1/gen.png">
You can view our General Knowledge page [here](https://cece-convo.xyz/#/general).

## Admin Log-in
Since the purpose of the chatbot is to provide users an easier and more efficient way to find the information that they are looking for, we decided to only include an admin login for our website. Users with the admin role will have access to the statistics of the application and the chatbot, as well as user feedback.

<img src = "./images/milestone1/admin_log.png">
You can view our Admin login page [here](https://cece-convo.xyz/#/signin).

## Admin Home Page
Once logged in, the admin user will now have a new item in the navigation bar called "statistics". This item will link the user to a statistics page, where all the stats of the site will be displayed.

<img src = "./images/milestone1/admin_home.png">
You can view our Admin Home page [here](https://cece-convo.xyz/#/). Please note that in order to view this page you must be logged in as an admin user. You can use the defauls credentials from our previous exercises to log in and view this page. 

## Statistics Page
The admin user is then brought to the statistics page after clicking on the navigation bar link. This page will display statistics such as user feedback on how they liked the chatbot. We plan on having our application display this information by having the use fill out a form after they have finished using the chatbot, and using a table to display the amount of ratings each specific question has.

<img src = "./images/milestone1/stats.png">
You can view our Statistics page [here](https://cece-convo.xyz/#/statistics). Please note that in order to view this page you must be logged in as an admin user.

# Developer Guide
 
First, [install Meteor](https://www.meteor.com/install):

Second, download a copy of [Hi-Covid-Convo](https://github.com/hi-covid-convo/hi-covid-convo) from Github.

Third, open up your terminal/command prompt and cd into the app directory of the Hi-Covid-Convo copy you had just downloaded
and install the necessary libraries by invoking meteor npm install:

```
$ meteor npm install
```

You must also install a pie chart library since our application will be using pie charts to display analytics. If this is not installed, then you won't be able to view the application. 

To do this, you can install the following libraries:

```
$ npm install underscore
````

and 

``` 
npm install react-minimal-pie-chart
```

After the libraries are installed, you can run the application by typing in the command:

```
$ meteor npm run start
```


The first time you run the app, it will create some default users that have been added to the database. Here is an
example of how the output may look:

```
I20201119-23:01:44.024(-10)? Creating the default user(s)
I20201119-23:01:44.024(-10)?   Creating user admin@foo.com.
I20201119-23:01:44.332(-10)?   Creating user john@foo.com.
I20201119-23:01:44.754(-10)? Monti APM: completed instrumenting the app
=> Started your app.
```

Note regarding bcrypt warning: You may also get a similar message when running this application:

```
=> Started proxy.                             
=> Started MongoDB.                           
W20201119-22:58:19.472(-10)? (STDERR) Note: you are using a pure-JavaScript implementation of bcrypt.
W20201119-22:58:19.515(-10)? (STDERR) While this implementation will work correctly, it is known to be
W20201119-22:58:19.516(-10)? (STDERR) approximately three times slower than the native implementation.
W20201119-22:58:19.516(-10)? (STDERR) In order to use the native implementation instead, run
W20201119-22:58:19.516(-10)? (STDERR) 
W20201119-22:58:19.516(-10)? (STDERR)   meteor npm install --save bcrypt
W20201119-22:58:19.516(-10)? (STDERR) 
W20201119-22:58:19.517(-10)? (STDERR) in the root directory of your application.
I20201119-22:58:20.471(-10)? Monti APM: completed instrumenting the app
=> Started your app.
```

On some operating systems (particularly Windows), installing bcrypt is much more difficult than implied by the above
message. Bcrypt is only used in Meteor for password checking, so the performance implications are negligible until your
site has very high traffic. You can safely ignore this warning without any problems during initial stages of
development.

If all goes well, the template application will appear at http://localhost:3000. You can login in using the credentials
in setting.development.json, or else you can register an new account.

Lastly, you can run ESLint over the code in the imports/directory with:

```
$ meteor npm run lint
```

# Community Feedback
We're interested in your experience using the application and would love to receive feedback. If you're interested in helping us improve the app, please take a few minutes to fill out [this form](https://forms.gle/Z9ALwHkicNkG6KU9A).


# Development History

If you would like to view our project history, as well as the completed issues from our first Milestone, view [HI Covid Convo M1](https://github.com/hi-covid-convo/hi-covid-convo/projects/1).

If you would like to view the issues and project history for the second Milestone, view [Hi Covid Convo M2](https://github.com/hi-covid-convo/hi-covid-convo/projects/2)
During this milestone we implemented more functionality into our application, which includes a form created for user feedback and displaying the statistics of that form in a analytics page that users with accounts may see. We also made adjustments to the visual design of the application with the goal of embracing the aloha spirit of Hawaii. We successfully configured our chat-bot Cece to answer up to fifty different questions regarding COVID-19, which will provide information and links to websites that users may find informative and useful.

If you would like to view the issues and project history for the third Milestone, view...

# Contact us
If you would like to contact the creators of HI Covid Chatbot, you can email us at the below addresses:

[Glen Larita](https://glarita.github.io/) - glarita@hawaii.edu

[Daniel Nilo](https://duhkneelow.github.io/) - dnilo@hawaii.edu

[Brian Abad](https://ba-bbage.github.io/) - babad8@hawaii.edu

[Sydney Dempsey](https://sydempsey.github.io/) - dempseys@hawaii.edu

