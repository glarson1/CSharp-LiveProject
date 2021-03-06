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

![Image controller and crud](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Third.PNG)

I then updated the database to create a table in the database to hold all things rentals which at the time didn't have any data inside yet, but in the image it has all the different tests that I tried to ensure things were running smoothly in other parts of the project.
![Image of db table](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Fourth.PNG)

### Story 3
This next story was to style the Create and Edit pages. I was given a list of styling wants and I applied them to those pages. Here is a before and after. There is also some hover effects on the buttons and click effects on the input boxes.
![Image of create before](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/FifthBefore.PNG)
![Image of create after](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/FifthAfter.PNG)

### Story 4
The task for this story was to create a dropdown on the Create and Edit pages for selecting on of the Rental types (Rental, RentalEquipment, and RentalRoom). Depending on what the user chooses in this dropdown will show/hide input fields in the form. For example if RentalEquipment is chosen, we would see the three fields for Rental and the three fields for RentalEquipment, without seeing the three fields for RentalRoom. This story is the story that challenged me the most, but also the story I appreciated the most because I got to learn so much from it. I started by adding an enum to my rental class

![Image of rental class with enum](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Sixth.PNG)

Then created variables of each field to be targeted in the form and passed in enum to the helper method DropDownListFor which creates a dropdown list that allows you to select between the different options that each render a different form.

![Image of rental class with enum](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Seventh.PNG)

Part of determining what was shown and what was hidden was done in the rent.js file. It would see what type of option the user selected (Rental, RentalRoom, RentalEquipment) and show what the user selected and hide what was not.

![Image of rental.js](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Eighth.PNG)

The rental type (Rental, RentalEquipment, RentalRoom) was determined in the controller. If someone entered in a value for PurchasePrice greater than 0, then that means that the rental type was RentalEquipment. If someone entered in a value for RoomNumber that was greater than 0, then the rental type was RentalRoom. The type "Rental" was always displayed and was displayed by itself when there were no values given for both PurchasePrice and RentalRoom.

![Image of rentalcontroller ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Nineth.PNG)

This is how it looked from the user side.

![Image of create page ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Tenth.PNG)
![Image of create page](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Eleventh.png)
![Image of create page ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Twelveth.PNG)
![Image of create page ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Thirteenth.PNG)

### Story 5, my last story of the 10 days
This last story wanted me to style the index page to give it a better layout using bootstrap. It also wanted the data to be displayed in a bootstrap card style, showing if the item was a choking or suffocation hazard. The data was to be organized into the correct options (Rental, RentalEquipment, RentalRoom).
This is what the index page looked like before starting the story.
![Image of old index page ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Fourteenth.PNG)

I began this story by getting the code for a bootstrap card inside of the cshtml page. Then I tweaked it to meet my needs and display what I wanted. I used three different foreach loops to go through all data from each of the three categories (Rental, RentalEquipment, RentalRoom) and display that data in the correct section. If statements were used to determine if the data was a choking hazard, suffocation hazard, or contained an entry for square footage. Also a placeholder image was used for all the cards during my time working on the story. In the future when the next team gets their hands on the project, the images will make more sense for each entry. 

![Image of old index page cshtml ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Fifteenth.PNG)
![Image of old index page cshtml ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Seventeenth.PNG)
![Image of old index page cshtml ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Eighteenth.PNG)

And here is the user side afterwards

![Image of new index page ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Sixteenth.PNG)
![Image of new index page ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Nineteenth.PNG)
![Image of new index page ](https://github.com/glarson1/CSharp-LiveProject/blob/main/Images/Twenty.PNG)



Overall I felt like the two weeks I spent working with the team on the project was very beneficial to my understanding of C# and .Net. 
