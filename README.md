# Alejandro Miranda's Portfolio
## Associate Software Engineer

Connect with me here on [LinkedIn](www.linkedin.com/in/alejandro-miranda-a69a7920a)

This portfolio showcases work I have been a part and some of the skills I have acquired along the way. This is not an exhaustive list but does give some light on the type of work I do.

## Table of Contents
  * [Introduction](#introduction)
  * [Technology I have worked with](#Technology-I-have-worked-with)
  * [ApplicationOwnership](#ownership)
  * [Projects](#projects)
    * [License The World](#License-The-World)
    * [Rocket Logic Toolbox](#rocket-logic-toolbox)
    * [Cascade Tool](#cascade-tool)
    * [Creating Custom Sonar Rules](#creating-custom-sonar-rules)
    
  * [Level Three Support/ Oncall](#Level-Three-Support/-Oncall)  
  * [Mentorship](#mentorship)
  * [Opportunities](#opportunities)
  * [Technical Excellence](#technical-excellence)

   
# Introduction

I started my journey to becoming a Software Engineer at Rocket Mortgage in the summer of 2021. I was on an IT Team which closely worked with some software engineers and after learning some C# on my own, I was given the greenlight start learning the basics between my regular work. After a short time I was able to spend all of my time working on the engineering work and thus transitioned into the world of software development. Finally, I was granted the title of Associate Software Engineer in July of 2022. My current team is 'Business Apllication Engineering' which is a level 3 support team for application AMP, and develops tools for various support areas.

# Technologies I have worked with
 * Progress OpenEdge ABL
 * JavaScript
 * TypeScript
 * Git / Github
 * Python
 * Angular
 * R Programming
 * HTML
 * CSS
 * C#
 * Java
 * SQL
 * Markdown
 * Rest API
 * GraphQL

# Application Ownership
## Primary SME
  * User Cascade Tool, AppID: 212165
  * AMP License Client, AppID: 213351
  * Loan Status Support Tools, AppID: 212156
## Secondary SME
  * Loan Status Framework, AppID: 213444
  * QuickClock AMP Integration, AppID: 210556

# Projects
  
## License The World
The decommissioning of CSA (Central Staging Area) on 6/28/23 required a new process to be created to pull all Bankers licenses into AMP from License the World as CSA was sending those licenses via BLING. This was a big project that required stages and strict testing. We created a class to effectively mirror the existing functionality but moved the source of truth from BLING to License The World. The new class pulls the data via a tidal job, twice a day, whereas the old method required AMP to have the licenses sent to it. 
The new class would be hitting an existing endpoints but I created methods in those endpoints. The first was a method to call License The World to get all banker licenses. The second was a method which called RHDS whenever we got back an NMLS we did not already have in AMP. I made the class call these methods so we would be able to write the licensing data to the database but much testing needed to be done to ensure AMP was receiving this data with the same results it used to get. Lower environment testing and query testing proved pivotal to the success of this project. 
The technologies used were: Progress, github, SonarQube

## Rocket Logic Toolbox
  *  [RL Toolbox UI](https://git.rockfin.com/BusinessApplicationEngineering/RL-Toolbox-UI) 
  *  [RL Toolbox BFF](https://git.rockfin.com/BusinessApplicationEngineering/RL-Toolbox-BFF)
The Rocket Logic Toolbox is a micro-frontend as a part of the overall Rocket Logic website. The toolbox is a User interface which allows the user to access the tools which take input from the user and perforn different tasks based on the tool selected. 

  
## Cascade Tool
### AppID: 212165
This tool solved a long time problem in AMP which required many hoops to be jumped through in a specific order to make changes to existing AMP user accounts which are connected to many loans. 
This tool is comprised of a few screens. The first screen takes in user input and validates if the input is acceptable. The second contains some backend work to find how many records are associated to the input while the screen lists the user functions associated with the input, which need to be verified to move to the next screen. 
The third screen allows the user to enter updates to all available fields. Lastly is a screen to ask if the user would like to update now or schedule for later in a tidal job.
The technologies used were: Progress, github, SonarQube


## Creating Custom Sonar Rules
  *  https://git.rockfin.com/AMP/custom-sonar-rules/pull/83

This is a custom Sonar rule which is implemented by sonarqube to detect and block users from storing email addresses in pop-up tables. A better method of storing emails has been created which is object oriented. This was a much needed upgrade which makes it much easeier to find emails that are stored in AMP and even easier to update emails in the future. 
The technologies used were: Java, Maven, Progress, html, and GitHub.
    
       
## Rocket Logic Toolbox
  *  [RL Toolbox UI](https://git.rockfin.com/BusinessApplicationEngineering/RL-Toolbox-UI) 
  *  [RL Toolbox BFF](https://git.rockfin.com/BusinessApplicationEngineering/RL-Toolbox-BFF)

# Level Three Support/ Oncall
A major part of being on Team Business Application Engineering is the work we do as a level three support team. There are many cases where AMP will not allow certain changes in a loan, whether that be because the loan is too far along in the process or the UI simply does not have a way to change that field. These instances require an engineer to find the location in AMP where the sreen or information is being looked at in the UI and find it in the backend. These fixes are critical to the business as loans cannot move forward without these changes. We as a team work quickly to resolve these issues, almost always resolving the issue the same day. 
I have taken it upon myself to answer those calls as soon as my work would allow, which has resulted in having resolved more of these issues than any other team member on my team. 
  
# Mentorship
As a part of my journey to becoming a Software Engineer I was given a mentor. My mentor and I were given a spreadsheet of things we should work through to solidify my confidence or introduce new ideas that are not part of my current work but I may see in my career. The mentorship lasted about six months and after the completion of the spreadsheet we parted ways.
I have since received another mentor with the intent to learn how to become a better engineer and to give overall career guidance. My current mentor is very focused on unit tests and how they can be optimized. I value mentorship as it is a great way to get information from people who have been through similar situations.
