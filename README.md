# Sample basic social media dataset
This repository is here for people who needs random social media data for some data manipulation, experimentation and data analysis.
This dataset is made of 6 CSV files (6 tables).

# Tables description

## User table
This table has been generated by using the website https://www.mockaroo.com/
It's pretty convenient and fast create fake data as long as you don't more than 1000 rows.
The rest of the tables will be generated with python script since there is some logic and connection to them.
![Image Not Found](https://lh3.googleusercontent.com/_Z5e0Y8421U6ekz-DEjyaB9jgBw1EPw-ynGc8ZNAUzeyE-9O1TuOLWqfGdYiSAQjXQw)


## Friendship table
This table contains information about user and their friends ID (or the person they follow). 
This script has been code assuming that the friendship in this social media in uni-directional, you can be friend with someone, but the person is not necessarily friend with you. It's more similar to Instagram or Twitter than Facebook in that sense.
<img src="img/friendship.png" width="300"

## Friend/Follow sent invitation table
This table contains data about all the friend invitation that have been sent (the accepted, ignored and refused ones).
The time at which the request was made is also generated.
<img src="img/request_sent.png" width="300"

## Friend/Follow accepted invitation table
This table contains data about all the friend invitation that have been accepted by the users.
The time at which the request was made is also generated.
<img src="img/request_accepted.png" width="300"

## Videos shared table
This table contains all the IDs of the video that have been shared to the social media by users. 
The time and the video duration are also generated.
<img src="img/video.png" width="300"

## Users interaction with the videos
This table content all the interaction with the video shared by the users. You can find information about who likes what videos and how long they spend interacting with it.
<img src="img/interaction_video" width="300"
