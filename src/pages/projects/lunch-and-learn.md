---
layout: ../../layouts/MarkdownProjectLayout.astro
title: 'Lunch & Learn'
description: 'REST API for getting recipes and learning resources for any country'
link: false
projectType: 'Solo'
image: 
  url: '/assets/project_pics/lunch-and-learn.gif' 
  alt: 'Screenshot of merchant dashboard' 
skills: ["Ruby on Rails", "ActiveRecord", "Postman", "PostgreSQL", "REST API", "VCR & WebMock"]
pubDate: 2023-05-14
author: 'Joe K'
repository: 
  backend: 'https://github.com/this-is-joeking/tea_party_api'
  frontend: false
  monolith: false
---
## About Lunch & Learn
This RESTful API is a back end service for getting recipes and learning resources from different countries. I created endpoints that allow a client to:
- Get recipes for a given country
- Get recipes for a random country
- Get learning resources for a given country
- Register a new user (generates an API key)
- Add a recipe to users favorites (requires user's API key)
- Get a users favorites (requires user's API key)


## My learning goals for this project were:
- Expose an API that aggregates data from several external APIs
- Expose an API that requires an authorization token
- Expose an API for CRUD functionality
- Determine completion criteria based on the needs of other developers
- Test API consumption/exposure using VCR and Webmock
