---
layout: ../../layouts/MarkdownProjectLayout.astro
title: 'Tea Party API'
description: 'REST API for Tea Subscription Service'
link: false
projectType: 'Solo'
image: 
  url: '/assets/project_pics/TeaPartyAPI.gif' 
  alt: 'Screenshot of merchant dashboard'
skills: ["Ruby on Rails", "ActiveRecord", "Continuous Integration", "PostgreSQL", "REST API"]
pubDate: 2023-05-14
author: 'Joe K'
repository: 
  backend: 'https://github.com/this-is-joeking/tea_party_api'
  frontend: false
  monolith: false
---
## About Tea Party API
This RESTful API is a back end service for a tea subscription company. It offers clients the ability to send a request to get all subscriptions for a given customer, create a new customer subscription, or deactivate a customer subscription. And it includes error handling if an invalid id is passed in a given request.


## My learning goals for this project were:
- Practice database design and defining model relationships
- Utilize advanced routing techniques including namespacing
- Practice exposing REST API
- Practice Continuous Integration with a code coverage report