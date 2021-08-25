# :soccer: Football Stats App - frontend

## General Informations
This repo contains frontend of Football Stats App. It is a server-side rendering (SSR) web application which help users to get data about matches results, the football schedule, as well as statistics of the best football teams. Read more about the application in two others repo of this project ([scrapers](https://github.com/Lasek25/football_stats_app_scrapers) and [backend](https://github.com/Lasek25/football_stats_app)).  
Feel free to test Football Stats App here (sometimes first loading may take a few seconds): [https://footballstatsapplication.herokuapp.com](https://footballstatsapplication.herokuapp.com)

## Tech Stack
* [Nuxt.js](https://nuxtjs.org/) - Vue.js framework (version: 2.14.6)
* [Nuxt.js PWA](https://pwa.nuxtjs.org/) (version: 3.0.2)
* [Nuxt.js Apollo](https://github.com/nuxt-community/apollo-module) - Nuxt.js module to use vue-apollo (version: 4.0.1-rc.5)
* [Vuetify](https://vuetifyjs.com/en/) - Material Design Framework for Vue.js (version: 2.5.3)
* [VeeValidate](https://vee-validate.logaretm.com/v3) (version: 3.4.5)

## Features
1. Main features:
    * get matches schedule and results
    * get informations about selected league - standings, results, fixtures, statistics of the teams (goals, corners, fouls, offsides, etc.)
    * get informations about the best teams in selected stats category (goals, corners, fouls, offsides, etc.)
    * sort and filter the above-mentioned data
2. Authorization:
    * create an account
    * sign in/out
    * change username or password
3. Others:
    * change theme of the application (dark or light mode)
    * enjoy fully responsive app on all of your devices (computers, smartphones and tablets)

## Instalation
1. Download or clone this repo with git clone `https://github.com/Lasek25/football_stats_app_front.git` command
2. Run command `yarn install` to install all dependencies
3. You can test application with official API (first `httpEndpoint`) or locally (second `httpEndpoint`, you should first install [backend of Football Stats App](https://github.com/Lasek25/football_stats_app)). Comment chosen line in `nuxt.config.js`:
```
apollo: {
    clientConfigs: {
      default: {
        // httpEndpoint: 'https://apifootballstatsapp.herokuapp.com/graphql',
        httpEndpoint: 'http://127.0.0.1:8000/graphql',
      }
    },
  },
```
4. Finally run app using `yarn run dev` command

## Usage
Football Stats App is ready to use (sometimes first loading may take a few seconds): [https://footballstatsapplication.herokuapp.com](https://footballstatsapplication.herokuapp.com). You can also download application to your smartphone, open your browser’s settings and tap *Add to home screen* (only for android users).
