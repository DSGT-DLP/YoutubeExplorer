# Assignment Instructions

As you saw in the README.md, your task is to build a React.js application that allows you to input the name of a Youtube Channel and display a table containing information about the constituent videos. For example, if I input "Mr. Beast" as the Youtube Channel in the search bar, I should be seeing a table containing videos Mr. Beast posted along with some high level information such as likes, views, comment count, publish date, etc


## What to do

As per the directions, we want our app to allow for the user to enter in the name of a Youtube Channel and a table should display with the associated videos. For each video, the information to show are the following:
* Title of Video
* Publish Date
* Description of video
* Number of views
* Number of likes
* Number of dislikes
* Number of comments

With that goal in mind, we need a good plan of attack so that we can prevent some roadblocks on this project. In an app, we usually can view it as the user view glued with the data handling aspect. The user view as the name implies is what the user can see and do on the app. The data handling aspect (AKA the backend) helps to execute on the user's actions in the app and interfaces with the internal data. 

See this diagram:

![frontend/backend](https://www.altexsoft.com/media/2020/01/word-image-67.png)

### Build the frontend (ie: what does the user see on the website?)
Try taking the instructions from above and seeing if you can brainstorm what a minimum viable experience should look like. If you are overthinking this, you are going in the wrong direction.

Hint: Think about this app like a search engine! What does the user do on a search engine?

You will want to follow the `FRONTEND.md` file for more information on how we can build out the frontend

### Build the backend (ie: how do we get the data for a given Youtube Channel from Youtube's server?)
Fortunately, Youtube provides what's called an API (Application Programming Interface). The best way to understand what an API is is through a real world example.

**Scenario:** Suppose you go to Starbucks to get your morning cup of coffee (let's say it's a Latte :)). When you go to place your order for a latte, the barista would take your order and whip up your latte (combining the coffee beans, milk in the right proportions to get the latte taste). You as the customer don't have to necessarily worry about how the latte is prepared, but rather that you receive the latte. This idea is called abstraction. We are not caring too much about the details of how your latte is prepared. Rather, we care about how to get a latte from Starbucks by placing the request and the barista is servicing it. This concept is exactly what an API is doing. 

**What's the advantage of an API:** On the developer's side, having a convenient way to fetch the data we want for our Youtube Explorer app would make our lives easier. We don't have to worry about the internal data modeling of Youtube videos because we have a convenient endpoint to place our "request" to and receive our items (kind of like placing an order for a latte and receiving that warm cup of coffee in your hand).

See this diagram below to understand how an API fits into an application:

![api-image](https://lvivity.com/wp-content/uploads/2018/07/how-api-work.jpg)

You will be following `BACKEND.MD` for this segment of the project

### Written component of the project
If you got to this step and have a working application, give yourself a pat on the back. You just completed your first full stack application project in React.js. To make sure that you understand how React.js works, please answer the questions in `WRITTEN.MD` **in your own words with 3-4 sentences maximum per response**

