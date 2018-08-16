# LIRI-Application

## What it des

LIRI is like iPhone's SIRI. However, while SIRI is a Speech Interpretation and Recognition Interface, LIRI is a _Language_ Interpretation and Recognition Interface. LIRI will be a command line node app that takes in parameters and gives you back data.

## Main Function

This is a command line node application where you can enter the following command in the terminal: 1. To search OMDB for a movie title: node liri.js movie-this <movie title> 2. To search Spotify for a song title: node liri.js spotify-this-song <song title> 3. To see the last 20 of my Twitter tweets: node liri.js my-tweets 4. For a random search: node liri.js do-what-it-says

## NPM Node Package Manager libraries are used

You will need to install the following npm libraries to get the app working:
npm install twitter
npm install --save node-spotify-api
npm install request
npm install omdb
npm install dot env

## Environment Variables

.env file is used to hold my twitter and spotify keys which hides them so they cannot be used. Therefore in order to get the application running you will need to create an .env file an use your own keys for Twitter and Spotify.

## Functions Explained

1. Search OMDB for a movie title:
   -executed by entering the follwing in the terminal
   node liri.js movie-this <movie title>
   -by putting in a movie title it will search the OMBD library and provide the following information regarding the movie title:
   -title of movie
   -year movie came out
   -IMBD rating
   -Rotten Tomatoe Rating
   -Country where movie was produced
   -Langauge
   -Plot
   -Actors

2. search Spotify for a song title:
   -executed by entering the following in the terminal
   node liri.js spotify-this-song <song title>
   -put entering a song title the application will searc Spotify Library and provide the following information related to te song:
   -Artist
   -Song Name
   -Preview Link
   -Album the song is from


    3. see the last 20 of my Twitter tweets:
        -executed by entering the following in the terminal
          node liri.js my-tweets
        -by entering this command in the terminal. It will display the last 20 tweets (if available) for the screen name in the application. For this application I have used my screen name 'GianlucaTORONTO'. As a result it will display my latest tweets.

    4. For a random search:
      -executed by entering the following in the terminal
        node liri.js do-what-it-says
      -by entering the line above in the command the application will take the information in the random.txt file which is <spotify-this-song,"I Want it That Way"> and execute it. Therefore the application will then run the spotify-this-song command for the song title "I Want it That way" and display the spotify informtion for this song. As a result in the random.txt file additional/different command can be added as required.

## Logging Activity

All activity and results are logged in the log.txt file.
