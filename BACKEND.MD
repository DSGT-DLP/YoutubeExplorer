# Youtube Explorer Backend
Now that we have the basic workings for how the user will interact
with our application, it's time to focus on how we will get the video data.

As mentioned in the [ASSIGNMENT.MD](ASSIGNMENT.MD) file, the user enters a Youtube Channel and we need to list out the videos in the given Youtube Channel. This task is where the Youtube API will come in handy


## What do we exactly need from the Youtube API?
Given a channel, we need the Youtube API to give us the list of the associated videos. For each video, we should get the following information:

1. Title of Video
2. Publish Date
3. Description of video
4. Number of views
5. Number of likes
6. Number of dislikes
7. Number of comments

## API 101
When we want to use an API, we would call what's called an **endpoint**. An **endpoint** is a fancy word for a dedicated URL that we talk to in order to get data we want. 

**Scenario**: If you want to order coffee from Starbucks, you would be telling the barista "I would like a latte". In computers, we would translate this sentence to something like `PUT https://starbucks.com/order?item=latte`. In this URL, we want to order coffee from Starbucks, so we hit the `starbucks.com` site, but we want to place an order, so we route to the `order` page. The `item=latte` part is a way of telling starbucks.com that the item we want is a latte. I'm simplifying a bit, but this should give you the main idea of what we can do with the Youtube API. 

Before we can even start using an API, we need to generate what's called an `API Key`. This is an identifier that should **not be shared/exposed to the world** which allows us to connect to the API/service. So, in the case of the Starbucks scenario, we could present some sort of account info (ie: rewards number, phone number, etc), greet the barista, etc before we can order that latte. Think of the API Key as your "badge". You don't want to expose your "badge" to any random person because unpleasant stuff could happen.

## Youtube API Instructions (based off of this [article](https://blog.hubspot.com/website/how-to-get-youtube-api-key))
1. Go to the [Google Developers console](https://console.developers.google.com)

2. Go to the top left corner of the website. You will see a drop down right next to the "Google Cloud Platform" text. Click that dropdown and select "Create Project". You don't need to enter an organization for the project. Give your project a handy dandy name

3. After you click "Create", you will see a dashboard. Click "Enable APIs and Services"

4. Select "Youtube Data API v3" (or whichever it says "Youtube Data API") from the "API Library" view

5. Click "Enable" to enable the Youtube Data API

6. You will be taken to an overview page and in the top right, you will see a button called "Create Credentials". Click that

7. Select "Youtube Data API V3" (or "Youtube Data API"). Select "Web server" for the question regarding "Where will you be calling the API from?". Select "Public Data" for "Which data will you be accessing?"

8. Click the blue button at the bottom and you will see an icon saying "Here is your API Key". Please copy and paste this API key to the `.env` file under `src/` (fill in the `YOUTUBE_API_KEY` variable). The `.env` file will safely store your API key and not expose it to other users. 

## Developing the Backend
Now that you have the API key generated for the Youtube API, we can start to interact with the Youtube API to get Youtube videos associated with a given Youtube Channel. 

For simplicity, your Youtube API code will be written in `YoutubeAPI.js` file under `src/` directory. There are a couple functions you can fill out here as a starting point to help you get the data you need to build that table!

## Tips
>Read the Youtube API documentation to make sure you understand how you are supposed to create the request to get the data you want from the Youtube API
>Filling out the functions in the `YoutubeAPI.js` might help break your problem down into manageable chunks
>Think about the format in which you want to send your data from the `YoutubeAPI.js` file to your frontend. JSON tends to be the standard format for such practice
