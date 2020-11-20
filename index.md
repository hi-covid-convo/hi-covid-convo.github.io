## Table of contents

* [Overview](#overview)
* [Goal](#final-outcome-of-the-application)
* [User Guide](#user-guide)
* [Developer Guide](#developer-guide)
* [Community Feedback](#community-feedback)
* [Development](#development)
* [Contact Us](#contact-us)

## [Hi-Covid-Convo Site](http://167.99.174.175/)

## Overview
Welcome to HI-Covid-Convo! The goal of this project is simple. We're aiming to provide an easy-to-use chat-bot for those concerned with COVID-19. Whether it's directly answering user's questions, or redirecting them to useful resources, we hope to give all users peace of mind.
[To hi-covid-convo repo](https://github.com/hi-covid-convo/hi-covid-convo)

## Goal of the Application
Over the next month, we plan to improve upon the applications functionality. By the end, our goal is to have a working chat-bot that will be able to answer COVID-related FAQs. Along with being able to parse user input and determine the best response/resource to provide, we also would like to include other resources on the site that will provide general information on COVID and how to remain safe during this pandemic. Because we want the site to remain anonymous, we plan to collect feedback statistics from users who use the chatbot. These statistics would include the most commonly asked questions, as well as how happy users are with the quality of the responses. These statistics would be available to an admin user once logged into the application.

# User Guide
### Our Current Progress..

## Landing Page
Users will first be taken to the landing page which will give an overview of the application. There is also a button to take them to Cece, the COVID chatbot. This page also discusses the goal for this application, and directs the user to go to the About page if they want to learn more

<img src = "./images/milestone1/landing.png">
You can view our landing page [here](http://167.99.174.175/#/).


## Cece the Chatbot
The button on the landing page will then take users to the Cece chatbot page. The page has a brief introduction to our chatbot Cece and some instructions on how to use it. On the right side of the screen is where the user will be able to enter in a question (as of now, the chatbot is still in progress and not fully complete).

<img src = "./images/milestone1/cece.png">
You can view our Cece Chatbot page [here](http://167.99.174.175/#/Cece).


## About Page
If the user wants to learn more about our application and its goal, they can visit the About page via the navigation bar. In this page we briefly go over what our goal is, and our purpose for creating this application.

<img src = "./images/milestone1/about.png">
You can view our About page [here](http://167.99.174.175/#/about).


## General COVID Info Page
The General knowledge page provides the user any general knowledge information about COVID-19. This includes topics like symptoms of the virus, how it is spread, and prevention and protection. This information was gathered from the [Centers for Disease Control and Prevention (CDC)](https://www.cdc.gov/coronavirus/2019-ncov/index.html). The General knowledge page is currently still in progress as well.

<img src = "./images/milestone1/gen.png">
You can view our General Knowledge page [here](http://167.99.174.175/#/general).

## Admin Log-in
Since the purpose of the chatbot is to provide users an easier and more efficient way to find the information that they are looking for, we decided to only include an admin login for our website. Users with the admin role will have access to the statistics of the application and the chatbot, as well as user feedback.

<img src = "./images/milestone1/admin_log.png">
You can view our Admin login page [here](http://167.99.174.175/#/signin).

## Admin Home Page
Once logged in, the admin user will now have a new item in the navigation bar called "statistics". This item will link the user to a statistics page, where all the stats of the site will be displayed.

<img src = "./images/milestone1/admin_home.png">
You can view our Admin Home page [here](http://167.99.174.175/#/). Please note that in order to view this page you must be logged in as an admin user. You can use the defauls credentials from our previous exercises to log in and view this page. 

## Statistics Page
The admin user is then brought to the statistics page after clicking on the navigation bar link. This page will display statistics such as user feedback on how they liked the chatbot. We plan on having our application display this information by having the use fill out a form after they have finished using the chatbot, and using a table to display the amount of ratings each specific question has.

<img src = "./images/milestone1/stats.png">
You can view our Statistics page [here](http://167.99.174.175/#/statistics). Please note that in order to view this page you must be logged in as an admin user.

# Developer Guide
 
First, [install Meteor](https://www.meteor.com/install):

Second, download a copy of [Hi-Covid-Convo](https://github.com/hi-covid-convo/hi-covid-convo) from Github.

Third, open up your terminal/command prompt and cd into the app directory of the Hi-Covid-Convo copy you had just downloaded
and install the necessary libraries by invoking meteor npm install:

<img src="images/milestone1/npminstall.png">

After the libraries are installed, you can run the application by typing in the command "meteor npm run start":

<img src="images/milestone1/npmrunstart.png">

The first time you run the app, it will create some default users that have been added to the database. Here is an
example of how the output may look like:
<img src="images/milestone1/creatingdefaultsM1.png">

Note regarding bcrypt warning: You may also get a similar message when running this application:

<img src="images/milestone1/bcrypt.png">

On some operating systems (particularly Windows), installing bcrypt is much more difficult than implied by the above
message. Bcrypt is only used in Meteor for password checking, so the performance implications are negligible until your
site has very high traffic. You can safely ignore this warning without any problems during initial stages of
development.

If all goes well, the template application will appear at http://localhost:3000. You can login in using the credentials
in setting.development.json, or else you can register an new account.

Lastly, you can run ESLint over the code in the imports/directory with:

<img src="images/milestone1/runlint.png">
# Community Feedback

# Development

If you would like to view our project history, as well as the completed issues from our first Milestone, view [HI Covid Convo M1](https://github.com/hi-covid-convo/hi-covid-convo/projects/1).

If you would like to view the issues and project history for the second Milestone, view [Hi Covid Convo M2](https://github.com/hi-covid-convo/hi-covid-convo/projects/2)
We plan on cleaning up the look of our application by implementing more colors and functionality for the chatbot and statistics features, so stay tuned!

# Contact us
If you would like to contact the creators of HI Covid Chatbot, you can email us at the below addresses:

[Glen Larita](https://glarita.github.io/) - glarita@hawaii.edu

[Daniel Nilo](https://duhkneelow.github.io/) - dnilo@hawaii.edu

[Brian Abad](https://ba-bbage.github.io/) - babad8@hawaii.edu

[Sydney Dempsey](https://sydempsey.github.io/) - dempseys@hawaii.edu

