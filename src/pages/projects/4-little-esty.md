---
layout: ../../layouts/MarkdownProjectLayout.astro
title: 'Little Esty Shop'
description: 'Merchant and Admin Tool for fictional ecommerce site'
link: 'https://intense-chamber-60518.herokuapp.com/admin'
projectType: 'Group Project'
image: 
  url: '/assets/project_pics/LittleEsty.gif' 
  alt: 'Screenshot of merchant dashboard'
skills: ["Ruby on Rails", "ActiveRecord", "Data Migration", "PostgreSQL", "Heroku", "SQL"]
pubDate: 2023-05-14
author: 'Joe K'
repository: 
  backend: false
  frontend: false
  monolith: 'https://github.com/this-is-joeking/bulk-discount'
---
## About Little Esty Shop
Little Esty Shop was created by four back end developers. It is a fictitious e-commerce platform where merchants and admins can manage inventory and fulfill customer invoices. We built the application with Ruby on Rails, and focused our learning on advanced routing, rake tasks that read csv files loading them into our database, complex ActiveRecord queries, simple consumption of [Nager.Date API](https://date.nager.at/swagger/index.html), and basic CRUD funtionality while maintaining MVC standards. Our Database uses many different relationships (many-to-many, one-to-many).

## My Contributions 
For this application I wrote several of the complex ActiveRecord queries such as calculating the total revenue (for all merchants and for a given merchant) on an invoice after any applicable bulk discounts are applied. This required use of subqueries and a combination of ActiveRecord and SQL.

## My learning goals for this project were:
- Practice database design and defining model relationships
- Utilize advanced routing techniques including namespacing
- Practice consuming a public API