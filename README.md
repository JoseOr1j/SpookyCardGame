# SpookyCardGame

A web app for visualizing personalized Spotify data

Built with a bunch of things, but to name a few:

Spotify Web API
Create React App
Express
Reach Router
Styled Components
Setup
Register a Spotify App and add http://localhost:8888/callback as a Redirect URI in the app settings
Create an .env file in the root of the project based on .env.example
yarn && yarn client:install
yarn dev
Deploying to Heroku
Create new heroku app

heroku create app-name
Set Heroku environment variables

heroku config:set SPOTIFY_CLIENT_ID=XXXXX
heroku config:set SPOTIFY_CLIENT_SECRET=XXXXX
heroku config:set REDIRECT_URI=https://app-name.herokuapp.com/callback
heroku config:set FRONTEND_URI=https://app-name.herokuapp.com
Push to Heroku

git push heroku master
Add http://app-name.herokuapp.com/callback as a Redirect URI in the spotify application settings

Once the app is live on Heroku, hitting http://app-name.herokuapp.com/login should be the same as hitting http://localhost:8888/login
