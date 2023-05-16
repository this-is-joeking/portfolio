---
layout: ../../layouts/MarkdownProjectLayout.astro
title: 'StreamLined'
description: 'GoodReads for movies and TV shows'
link: 'https://stream-lined.herokuapp.com/'
projectType: 'Group Project'
image: 
  url: '/assets/project_pics/streamlined.gif' 
  alt: 'Screenshot of homepage'
skills: ["Ruby on Rails", "REST API", "Bootstrap", "OAuth", "Heroku", "VCR & WebMock", "Circle CI", "RSpec", "Service Oriented Architecture", "CSS", "PostgreSQL", "Postman"]
pubDate: 2023-03-14
author: 'Joe K'
repository:
  backend: 'https://github.com/Streamlined-Turing/streamlined_be'
  frontend: 'https://github.com/Streamlined-Turing/streamlined_fe'
  monolith: false
---
## About StreamLined
StreamLined was built by a team of 6 backend developers. It is a tool to track movies and TV shows a user would like to watch, are currently watching, and track media a user has watched. Once a user has created a StreamLined account, they can access a dashboard with three default lists to categorize their media: 'Currently Watching,' 'Want to Watch,' and 'Watched.' Additionally, the user can search for movies and TV shows by title, view the media details, and save to the appropriate list in their dashboard. Once a user has finished watching their show or movie, they can provide reviews and ratings. In future iterations of this application, users of this app will be able to add their streaming services to their profile and search for their desired media based on the streaming service available to the user.

## My Contributions
My role on this project was to start the back end by consuming the Watchmode and TMDB APIs and exposing the first few endpoints, including the search media endpoint. After a five-day sprint on the back end, I pivoted to the front end and focused on styling. Since I am primarily a backend developer, many projects I built as a beginner looked like Craigslist. As great as Craigslist is, I was excited to have the opportunity to make a more visually pleasing site.

## My learning goals for this project were:
- Self-teach and implement Twitter Bootstrap for cohesive styling across the application
- Utilize VCR with WebMock
- Build web application that uses service-oriented architecture
- Consume multiple REST APIs

## Challenges
Since we were building the front end at the same time as the back end, it was crucial to establish a JSON Contract early. It took some time to determine what the back end would need to provide the front end. Once we set the contract, we quickly ran into an issue with the rate limit on the Watchmode API. We promptly pivoted to add The Movie Database as an additional data resource. The Watchmode API is still used but for far fewer requests.