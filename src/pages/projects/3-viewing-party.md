---
layout: ../../layouts/MarkdownProjectLayout.astro
title: 'Viewing Party'
description: 'Tool for planning and inviting friends to a movie viewing party'
link: 'https://movie-viewing-party.herokuapp.com/'
projectType: 'Partner Project'
image: 
  url: '/assets/project_pics/vp.gif' 
  alt: 'Screenshot of users dashboard'
skills: ["Ruby on Rails", "REST API", "Bootstrap", "Authorization & Authentication", "Heroku", "CI CD", "RSpec", "VCR & WebMock", "ActiveRecord", "PostgreSQL"]
pubDate: 2023-01-14
author: 'Joe K'
repository: 
  backend: false
  frontend: false
  monolith: 'https://github.com/this-is-joeking/viewing_party_lite'
---
## About Viewing Party
Viewing Party is a web application for creating and inviting friends to a movie viewing party. It consumes the Movie Database API for all movie data. Viewing Party uses a service facade pattern to abstract logic from the controller.

## My Contributions
I implemented authentication and authorization using BCrypt to store passwords as hashes in our database. Additionally, I implemented Bootstrap to improve styling. I also used this application to practice implementing codecov so that a coverage report automatically generates for any pull requests and a badge with current coverage renders on the repository.
Initially, we used WebMock for testing, but I refactored to use VCR with WebMock so that fixture files automatically update when you delete the cassette and re-run the test suite.

## My learning goals for this project were:
- Authentication/authorization using BCrypt
- Consume REST API that requires authentication
- Test consumption of APIs
- Implement Service Facade Pattern
- Implement VCR
- Use Rubocop for code quality / linting