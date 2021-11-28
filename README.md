# CSharp-LiveProject
## Introduction
The last two weeks of my time spent at The Tech Academy, I worked on an MVC web application in C# for a theatre in Portland. The website was split into sections that the theatre wanted. Those sections were rentals, production, and a blog section. In this project I worked in a team of fellow students for the rental based section of the site. The team communicated through Discord, and project management was carried out using Azure DevOps. Throughout the project I worked on both the front end and the back end to complete my stories and continue progress of the application. The things I learned on this project I believe will be put to use on many future project whether or not those projects use the same stack or not.
## Overview
### Story 1
My first story of the project was to create a method that can be used to limit the number of words displayed using ellipses. For example, "Lorem Ipsum Lorem Ipsum Lorem Ipsum" would turn into "Lorem Ipsum Lorem...". This way the user can still type all that they want but it wouldn't be displayed in a way that would take over the entire page. The method that I came up with was this
![Image of word limiter](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/First.PNG)

### Story 2
The next story I was tasked with was to create an entity model for the Rental class so that rentals could be saved to the database. The first thing I did was create the Rental class where I also created the RentalEquipment and RentalRoom classes that inherited from Rental.
![Image of rental class](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Second.PNG)

The next thing I did was create the controller and scaffolded the CRUD pages for it.

![Image of rental class](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Third.PNG)

I then updated the database to create a table in the database to hold all things rentals which at the time didn't have any data inside yet, but in the image it has all the different tests that I tried to ensure things were running smoothly in other parts of the project.
![Image of rental class](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Fourth.PNG)

### Story 3
This next story was to style the Create and Edit pages. I was given a list of styling wants and I applied them to those pages. Here is a before and after. There is also some hover effects on the buttons and click effects on the input boxes.
![Image of rental class](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/FifthBefore.PNG)
![Image of rental class](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/FifthAfter.PNG)
