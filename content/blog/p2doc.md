---
layout: layouts/post.njk
title: The Great Yodini (P2)
description: This is the documentation for my second class project
date: 2026-03-23
image: "../public/assets/GreatYodini.jpeg"
category: Project
tags: ["project"]
---
## The Great Yodini Live Site

For this project, my group and I were tasked to use an API for its unintended usage and incorporate a nedb database somehow. We decided to do a riff on the "Zoltar" fortune booths you see at fairs, and we mixed Yoda and fortune telling to get: The Great Yodini
<br><br>

**My group members' blogs:**
- [Judy's Blog](https://judyzhang05.github.io/web-design-blog/blog/7_project2/)
- [Shasuna's Blog]( https://shasunal.github.io/shasunagarden/blog/project2documentation/)

Project Repo **[link](https://github.com/shasunal/Yodini)**
<br>

Live Site **[link](http://167.172.146.126:3000)**
<hr>

## Takeaways

1. ### My role as the backend developer:

- For this project I was in charge of connecting the **[API](https://forismatic.com/en/api/?ref=apilist.fun)** to the project so that we could dispaly the quotes from the inspiration API. At first we were using a movie quote API, but due to a paywall we pivoted to using an inspirational quote API instead. It worked out in the end. 
- For the most part I used a lot of the class demos to structur the code for this project. I found using nunjucks made passing in the information from the database pretty easy. I will say github pull requests could be annoyign at times: when branches would time out/ sometimes we'd have merge issue because the data.db file had content
<br>

2. ### Some challenges I experienced:
- **Quote Dupliactes**
    - Some challenges I faced during this project was getting multiple quotes from the API. The API was beginner friendly which was helpful but I still ran into an issue where it would spit out the same three quotes to the database. Ideally the code was meant to pass in three separate random quotes from the API this was meant to be the "meanings" for each of their cards. However, I was using Math.random() in js and sometimes it would be just start passing in the same quote. So to fix that: each quote in the API is assigned a numeric key, so I tweaked the code to pull three random keys insteads. That way the chances of duplicates is lower. 

- **Fortune Bugs**
    -  Due to time constraints my group and I decided to simulate randomness. So we are pulling two things from the user: their name and their conecern. But we are giving them 5 things in return: their name, concern, 3 cards and their meaning, and a final verdict. The bug that arises comes form the fact that we didn't use cookies to spit this information back at them. We didnt feel comfortable using cookies. So instead, I just used database.render() to spit out the last entry to the databse. It worked for awhile but then it seemed that if we didn't empty out the database before a new entry it would spit out whatever was the last entry. To fix that issue I created a button that clears the database when the user finishes. However, there isn't any logic preventing the user to just click out the window and if they don't click the button then the bug may continue. So maybe in the future I could implement some sort of cookies functionality/ using the database "id" to spit out user-specific information instead.
 