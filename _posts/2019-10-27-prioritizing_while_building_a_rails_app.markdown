---
layout: post
title:      "Prioritizing while building a Rails App"
date:       2019-10-27 23:33:59 +0000
permalink:  prioritizing_while_building_a_rails_app
---


I spent a good amount of time mauling over all the specifications I have for my rails app and what I want it to look like. That time spent was me trying to mentally figure out "where to start?". It felt like there is so much to do and it dawned me how important as a beginner engineer it is to breakdown TO-DOs into smaller TO-DOs to segment my progress towards finishing the project.

### TL;DR: Do NOT try to do everything at once

Ok, now that we got the purpose of this blog out there - here is my story: 

I started out my app by making the mistake of wanting to do it all. I wanted to make this cool app that lets you keep track of all the info you need for your upcoming travel plans. I found myself wanting to make a model for lodgings, transportations, and things to do (on top of my regular user, trip, country, city models). Also, while accessing all kinds of APIs to get all this data, such as Google Calendar and Expedia.

Crazy, right? Yes, I admit it.

Well, that is what happens when you go into the rabbit hole. I went in so deep that it got out of control and had to scrap the entire app. So I went back to the ideation board... a bit... more humbled.


### At the ideation board

What do I want to build? 
What will my app do?
What are the specifications I need to meet for the project?

1. Drew it out on a paper what I envision it to look like from a user perspective.
2. Wrote out what models/tables I needed. *(at the most basic level)*
3. Created a flow chart on what the associations and relationships of these models.
4. Wrote out a list with all the steps I will have to do to in completing my application. *(this isn't the end all, you can always add more to this list AFTER basic specs are met)*

### Make steps for your steps


##### Large Step Sample (with smaller manageable steps)

**Create Users TO-DO**

What should my user model have?
A username, an email, and a password.

Easy? Right? WRONG.

A database for this information.
A gem that will keep my users' passwords secure.
Include columns needed to keep the passwords secure.
Drop into console to test out model/db are working properly and instantiating users.
Create controller file for my user model.
Create methods in controller file.
Add routes for users.
Create views for controller actions.
Create sign up form.
Implement a third party 'sign up'.
Add columns needed for the third party.
Add route for third party.
Add logic in controller to create new user.
Test that user will be able to create user and be redirected to show page.

**Move into the Sessions TO-DO**

My sessions to-do overlaps with my users to-do so the list continues. At this point it is important to follow the flow versus wanting to focus on all the other things you just remembered while doing the above list. Just move the item to the part of your flow it belongs in.


### Disclaimer

Building a full rails app is NOT easy. 


#### ...but

It helps extend one's knowledge past the materials already learned as it becomes challenging putting all the pieces together to this extent. Pace yourself. 


# Go us! 



