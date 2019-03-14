# Mappr Back End Homework

# Jarvis-Bot
#### Jarvis is not the Iron Man's butler. Jarvis will be a command line node app that takes in parameters and gives you back data.

## Description on how to use the app

 - Once cd-ing into the Jarvis-Bot directory, type in: node jarvis.js INSERTCOMMAND 
 - List of commands:
  1. my-tweets
  2. spotify-this-song
  3. movie-this
  4. do-what-it-says
 - If no song is typed in after the spotify-this-song, a default song will be searched. 
 - If no movie is typed in after the movie-this, a default movie will be searched. 
 
## Requirements

### What Each Command Should Do

1. `node jarvis.js my-tweets`

   * This will show your(or someones) last 20 tweets and when they were created at in your terminal/bash window.

2. `node jarvis.js spotify-this-song '<song name here>'`

   * This will show the following information about the song in your terminal/bash window
     * Artist(s)
     * The song's name
     * A preview link of the song from Spotify
     * The album that the song is from

   * if no song is provided then your program will default to
     * "New Rules" by Dua Lipa

3. `node jarvis.js movie-this '<movie name here>'`

   * This will output the following information to your terminal/bash window:

     ```
       * Title of the movie.
       * Year the movie came out.
       * IMDB Rating of the movie.
       * Country where the movie was produced.
       * Language of the movie.
       * Plot of the movie.
       * Actors in the movie.
       * Rotten Tomatoes Rating.
       * Rotten Tomatoes URL.
     ```

   * If the user doesn't type a movie in, the program will output data for the movie 'Mr. Nobody.'
     * If you haven't watched "Mr. Nobody," then you should: <http://www.imdb.com/title/tt0485947/>
     * It's on Netflix!

4. `node jarvis.js do-what-it-says`
   * Using the `fs` Node package, Jarvis will take the text inside of random.txt and then use it to call one of Jarvis's commands.
     * It should run `spotify-this-song` for "I Want it That Way," as follows the text in `random.txt`.
     * Feel free to change the text in that document to test out the feature for other commands.

### BONUS

* In addition to logging the data to your terminal/bash window, output the data to a .txt file called `log.txt`.

* Make sure you append each command you run to the `log.txt` file. 

* Do not overwrite your file each time you run a command.

- - -
