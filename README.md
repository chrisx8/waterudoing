# Water U Doing

[![build](https://github.com/chrisx8/waterudoing/workflows/build/badge.svg)](https://github.com/chrisx8/waterudoing/actions?query=workflow%3Abuild)
[![CodeFactor](https://www.codefactor.io/repository/github/chrisx8/waterudoing/badge)](https://www.codefactor.io/repository/github/chrisx8/waterudoing)

A fun and interactive way to know your weekly water consumption habits and compete with others on the leaderboard.

[BoilerMake VIII submission](https://devpost.com/software/water-u-doing)

## Inspiration

We were concerned by the ever-growing problem of water wastage around the globe and its impacts on the environment. We also drew heavy inspiration from ECOLAB's message of designing smart solutions for modern environmental problems. Our idea was to make the process of learning and spreading awareness about water consumption as engaging as possible.

## What it does

Our web app aims to give users the chance to compete with each other. Participants have to simply take a short evaluation about their weekly water consumption habits. Their responses are then carefully analyzed and compared to aggregated data to determine a score. This score is indicative of the number of gallons that the participant uses each week, and they are placed into one of four tiers based on the score. The users can compete and see each other’s scores via the leaderboard, from which they can determine who their conservation rivals are and view their profile data. 

## How we built it

We used Django (a Python-based web framework) to develop most of the back-end. Our data was stored using MySQL and SQLite and all the code was running in Docker containers, which are available on Docker Hub. Gunicorn served as a communicator between our web sever and our back-end code, while NGINX was used to serve and distribute the project over the web with proper HTTPS. Most of the front-end was written in HTML/JS/CSS, with the help of frameworks like Dug, Sass, and Bootstrap. We used GitHub and Slack to collaborate. 

## Challenges we ran into

- Domain.com (one of the teammates received browser errors (possibly due to rate limits), DNS propagation took much longer than usual)
- Form data collection and handling are unconventional (because we were not using standard HTML forms)
- Django DB migrations caused problems
- Latest static files not serving due to browser cache
- Development server crashing due to unknown reasons
- Writing an interactive multi-page form with styling
- Combining Node.js workflow was Django workflow

## Accomplishments that we are proud of

- Making input-validated (server-side and client-side) forms
- Creating ravishing interfaces
- Using Docker and Docker-compose for deployment
- Survived the spooky horror stories
- Were there for Iris' first bug
- Completing the project (mostly...)

## What we learned

- The importance of communication and dividing work between teammates
- HTML/JS/CSS

## What's next for Water-U-Doing?

- Daily, Weekly, and Monthly challenges
- Calculating usage for other forms of energy such as electricity and gas
- 2FA, third-party sign-in support (Google, GitHub, Microsoft)
