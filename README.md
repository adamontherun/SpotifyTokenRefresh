# SpotifyTokenRefresh

For apps that use the Spotify API, users are required to login once every 60 minutes unless you implement the Authorization Code flow. Using this flow requires that you setup your own server that performs a token swap and refresh. 

Use this quick deploy to Heroku for a one-click deployment of a free server that acts as your token swap/refresh service. You'll need to enter your Client ID, Client Secret and Callback URI. 

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

By default, this sets you up with a free server, which has the drawback that it goes to sleep after 30 minutes of inactivity. To keep your server alive, setup a service such as [StatusCake](https://statuscake.com) to ping your server once every ten minutes.