<img width="80%" src="img/readme-img.png"/>

# Sample basic social media dataset
This repository is here for people who needs random social media data for some data manipulation, experimentation and data analysis.
This dataset is made of 6 CSV files (6 tables).

## How to use the tool
At the root of the project, you can find 6 CSV files that have been generated for the following settings
- Users: 1000
- Minimum friends per user: 2
- Maximum friends per user: 20
- Date range : 1/1/2014 to 1/1/2016
- Maximum video shared by users: 50
- Maximum like got by videos: 100 

You can use the following script to generate new data with the configuration you like. Keep in mind that you should choose carefully your settings so you can don't have more friends or likes than actual users for instance.
```bash
python generate_data.py -users 1000 -minfriends 2 -maxfriends 20 -startdate '1/1/2014 1:00 PM' -enddate '1/1/2016 1:00 PM' -maxvideo 50 -maxlike 100
```

# Tables description

## User table
This table has been generated by using the website https://www.mockaroo.com/
It's pretty convenient and fast create fake data as long as you don't more than 1000 rows.
The rest of the tables will be generated with python script since there is some logic and connection to them. 

<img src="img/users.png" height="200">

## Friendship table
This table contains information about user and their friends ID (or the person they follow). 
This script has been code assuming that the friendship in this social media in uni-directional, you can be friend with someone, but the person is not necessarily friend with you. It's more similar to Instagram or Twitter than Facebook in that sense. 

<img src="img/friendship.png" width="200">

## Friend/Follow sent invitation table
This table contains data about all the friend invitation that have been sent (the accepted, ignored and refused ones).
The time at which the request was made is also generated. 

<img src="img/request_sent.png" width="400">

## Friend/Follow accepted invitation table
This table contains data about all the friend invitation that have been accepted by the users.
The time at which the request was made is also generated. 

<img src="img/request_accepted.png" width="400">

## Videos shared table
This table contains all the IDs of the video that have been shared to the social media by users. 
The time and the video duration are also generated. 

<img src="img/video.png" width="450">

## Users interaction with the videos
This table content all the interaction with the video shared by the users. You can find information about who likes what videos and how long they spend interacting with it. 

<img src="img/interaction_video.png" width="300">
