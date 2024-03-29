# Emotional APIs

## Goals

1. Create a RESTful API that uses IBM Watson and another API to perform tasks such as tone analyser on data from an outside source (Get creative!).
2. Become comfortable using 3rd party APIs such as [Watson](https://cloud.ibm.com/developer/watson/services).
3. Gain a better understanding of async in general as it relates to programming in JS.
4. Manipulate data you receive back from 3rd party APIs.
5. Understand that servers can communicate with other servers too - it doesn't have to be client/server.

## Instructions

- Before you begin, be mindful that we want to avoid pushing any sensitive data (such as API keys) to GitHub. To do so, you should only store secure credentials in a `config.js` file. You should then add `config.js` to your `.gitignore`.

### Morning

1. Sign up to [IBM Watson's](https://console.bluemix.net/) API. Create a free trial account with IBM Bluemix. Spend some time learning about how they work -> 
- [How does IBM Watson work? - Youtube](https://www.youtube.com/watch?v=r7E1TJ1HtM0)
- [IBM Docs](https://console.bluemix.net/catalog/?search=label:lite&category=ai)

2. Select and create your service from the [IBM catalog](https://console.bluemix.net/catalog/?search=label:lite&category=ai). A good one to get started is the [tone analyser](https://console.bluemix.net/catalog/services/tone-analyzer).

3. Once you have created your service, note down the `API key` and `url` - keep them secret, keep them safe.

4. Use the npm package [watson-developer-cloud](https://www.npmjs.com/package/watson-developer-cloud) to connect to IBM Watson's [tone analyser service](https://console.bluemix.net/catalog/services/tone-analyzer) (_**or whichever module you choose to use!**_). 

- _**Hint:**_ run your file using `node` and some hard coded data to test that you have it set-up correctly!

### Afternoon 

5. Select a second API that you can use with one of the IBM Watson services. Have a look through the API list provided and what data they have available. Feel free to explore and find another API that you can use, you're not limited to the ones here!

6. Make requests, using Insomnia, to your chosen API to see how requests should be made, and how it responds with data.

7. Build out your API, thinking carefully about how you might make your endpoints RESTful. Aim to implement a route that receives a data from an API and sends it to one of the Watson API services

- Feel free to go further and explore what IMB Watson is capable of. It also has modules that work with images and analyse them, which could be fun.

8. Build a front end for this application. (You could use [EJS](https://ejs.co/)!) Think about what kind of a UI you would need.

9. Host your app on heroku so the world can see your handy work!

## Useful API's

- [Twitter](https://developer.twitter.com/) (if you are lucky enough to get API keys!)
- [They Work For You](https://www.theyworkforyou.com/api/)
- [Google Books](https://developers.google.com/books/docs/overview)
- [News Api](https://newsapi.org/)
- [Trivia](http://jservice.io/)
- [Marvel Comics](https://developer.marvel.com/)
- [Twilio](https://www.twilio.com/)

Or, check out this [list](https://github.com/toddmotto/public-apis) of free APIs but make sure that you choose one that requires no auth _or_ just an api key.

## Some ideas for further development

- Cache the results in a SQL database (i.e. if an identical request to your API has already been made, retrieve the results from your database)

- Implement a route that uses two Watson API services

- Examples of previous students work
  - Use graphs to display information about a user's personality.
  - Use twilio to text username and then text back top 5 traits.
  - Which dictator your tweets relate most to.
  - How close your personality is to one of your friends.
  - A website that takes a twitter handle, gets their last tweet and converts it into a audio file translated into another language.
  - Reply to a twitter user with a different message depending on their personality stats from Watson

### This sprint is open-ended and is designed to make you:

1. Get creative and try to think of what you achieve with these tools.
2. To read through documentation and try to work out how to piece different apis together to achieve a desired outcome.

Most importantly, have fun!
