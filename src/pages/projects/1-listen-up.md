---
layout: ../../layouts/MarkdownProjectLayout.astro
title: 'Listen Up'
description: 'A sound quiz game!'
link: 'https://listenup-game.herokuapp.com/'
projectType: 'Group Project'
image: 
  url: '/assets/project_pics/listen-up.gif' 
  alt: 'Gif screen capture of game being played'
skills: ["Ruby on Rails", "GraphQL", "Postman", "Heroku", "GitHub Projects", "CI CD", "REST API", "VCR & WebMock", "RSpec", "ActiveRecord", "SQL", "Service Oriented Architecture", "Heroku", "Postman", "PostgreSQL"]
pubDate: 2023-05-14
author: 'Joe K'
repository:
  backend: 'https://github.com/Listen-Up-2210'
  frontend: 'https://github.com/Listen-Up-2210/listen-up-ui'
  monolith: false
---
## About Listen Up!
For this project I worked on a team with 7 other developers. 3 of us made up the back end team. Our backend is the core of the sound-guessing game that powers the app. It holds and manages data on the various sounds that the user can play, and responds to requests from the front end to generate decks of sounds and track scores on the leaderboard.

When the front end requests a new game, the backend randomly selects 8 sound cards from the available pool of sounds and combines them into a deck. This ensures that each game is unique and challenging.

Once the deck is created, the front end can request sounds from the deck until it is empty. The backend keeps track of the user's score after the game, so they can compare their scores across other players and their past games.

Overall, our backend provides a seamless and engaging user experience, with a variety of sounds and challenging gameplay that keeps users coming back for more.

For ease of use we added a [Graph*i*QL Playground](https://listen-up-be.herokuapp.com/graphiql)

This application loads data for the game via a rake task that uses the Google Sheets API to load the data from a Google Sheet where we input the ID of the sound from Freesound API along with the correct and wrong answers. We set it up this way so all team members could easily add more sounds/questions to the game. 

## My Contributions
As all three of us on the back end were learning and implementing GraphQL for the first time, we paired for most of the process. I took the lead initially, as I had done the most with GraphQL (a small YouTube tutorial). I also took charge of the documentation, including writing the README and documenting all queries/mutations within the repo and in Postman.
## My learning goals for this project were:
- Working with separate frontend and backend teams using agile methodologies
- Self teach and implement GraphQL
- Utilize PR templates and comments as part of managing git workflow
- Consume Google Sheets API
- Implement Continuous Integration & Continuous Delivery
- Focus on open and frequent communication across teams via Slack, Zoom, Miro board, & Github Project Board

## Challenges
In our original game architecture, we organized the application such that the front end would request all eight questions and sound URLs at the start of the game. In testing, we discovered this caused an unacceptable load time to start the game and posed a risk of reaching the Freesound API rate limit if multiple people started games simultaneously. Based on my suggestion, we corrected this by changing the structure so the front end would request one question/sound at a time, significantly reducing game load time and the likelihood of reaching our API rate limit of 60 requests per minute.