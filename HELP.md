### Before You Begin

1. Jarvis will display your latest tweets. If you don't already have an account on Twitter, make one and post a few tweets about your latest projects.

2. Make a new GitHub repository called jarvis-node-app and clone it to your computer.

3. To retrieve the data that will power this app, you'll need to send requests to the Twitter, Spotify and IMDB APIs. You'll find these Node packages crucial for your assignment.

   * [Twitter](https://www.npmjs.com/package/twitter)
   * [Spotify](https://www.npmjs.com/package/spotify)
   * [Request](https://www.npmjs.com/package/request)
     * You'll use Request to grab data from the [OMDB API](http://www.omdbapi.com).


### Instructions

1. Make a .gitignore file and add the following lines to it.


```
node_modules
.DS_Store
```

2. Make a JavaScript file named `keys.js`. **Do Not** add this file to the .gitignore. This would be a good thing to do in the real world, but it makes grading this assignment a challenge.

Inside keys.js your file will look like this:

```JavaScript
console.log('this is loaded');

exports.twitterKeys = {
  consumer_key: '<input here>',
  consumer_secret: '<input here>',
  access_token_key: '<input here>',
  access_token_secret: '<input here>',
}
```

3. Get your Twitter API keys by following these steps:

   * Step One: Visit <https://apps.twitter.com/app/new>
   * Step Two: Fill out the form with dummy data. Type `http://google.com` in the Website input. Don't fill out the Callback URL input. Then submit the form.
   * Step Three: On the next screen, click the Keys and Access Tokens tab to get your consume key and secret. 
     * Copy and paste them where the `<input here>` tags are inside your keys.js file.
   * Step Four: At the bottom of the page, click the `Create my access token` button to get your access token key and secret. 
     * Copy the access token key and secret displayed at the bottom of the next screen. Paste them where the `<input here>` tags are inside your keys.js file.

4. Make a file called `random.txt`.

   * Inside of `random.txt` put the following in with no extra characters or white space:
     * spotify-this-song,"I Want it That Way"

5. Make a JavaScript file named `jarvis.js`.

6. At the top of the `jarvis.js` file, write the code you need to grab the data from keys.js. Then store the keys in a variable.

7. Make it so jarvis.js can take in one of the following commands:

   * `my-tweets`

   * `spotify-this-song`

   * `movie-this`

   * `do-what-it-says`
