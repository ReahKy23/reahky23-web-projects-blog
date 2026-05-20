---
layout: layouts/post.njk
title: Interlinked
description: This is the documentation for my final class project
date: 2026-05-20
image: ".../public/assets/interlinked.png"
category: Project
tags: ["documentation"]
---

## Project Links
1. Live Project **[link](http://161.35.125.196:7001/)**


2. *Group Member's blogs:*
  - - Gabby's Blog Site **[link](https://gabasha00.github.io/gabs-web-design-blog/blog/project3/)**
  - - Ivy Blog Site **[link](https://portorfolio.github.io/blog/blog/project3/)**

## Project Overview

This general story behing our project, is that this automous computer, "Mutha" has been stranded in space for some time after a mission gone wrong killed its crew. It now floats across space aimlessly. This is the first time it has come in contact with a human (the user) in years. It wants the user to explain to it the meaning of man.

### Project Design Inspiration and Concept

### My Contributions

1. Project Repo and File set up
   - I was in charge of creating the repo for the project and the base layout. I imported the necessary libraries, created the njk views and templating for the main page routes.
2. Project prototype and design
   - I created a high-fidelity mockup of the goal interactions for this project. I had a more creative role in this project compared to Project 3. I had fun pulling differnet backgrounds and textures together to sell this "space" look. I think it also has an retroness to it that makes it look like it has been lost for years.
3. Front-end assets and interactions
   - Cookies
      - I integrated Express session and cookies into the site on the server.js so that each cookie is assigned a unique id. This was meant to be used for deleted capabilities, but that had to be tabled due to git conflicts. However, the server.js would check to see if a cookie exists for that user. If a cookie exists the "contribute" and "explore" button will show because the user would already know the background story of the site. 
      If a cookie does not exist those buttons will be hidden and the user will have to click on the computer to navigate through the site. Then on reload the buttons will appear. 
   - Html Form
      - I did the the html and css for the html form. I also connected the values on the backend so that the information will pass into the post nedb database. 
   - Map text overlay
      - I did the js for the text overlay that happens when a user's post includes the optional caption. I really like this detail because it breaks up the modal and makes the project feel as though it takes up more space on the screen.
   - Overall Site Css

### Project Challenges

1. Git being Git
   - we were supposed to have a cookies implementation that would allow users to delete their post/star if the unique session id matched. However, git started giving us trouble and the star nodes were very sensitive. Though I would have loved to have had that feature, I think that is something that can be added in future iterations of this project. 
### Future Iterations

1. Sound elements, It would be cool if there was a sound element in the back of the window
2. I think a timed animation that hints to the user to click/ move mouse onto the computer.
3.  Including the cookies and express sessions to manipulate the viewports returning users have in
4. It would be really cool to implement a virtual keyboard. I did have one called kioskboard and it was working in terms of the text showing up on screen and in the database on the back end. The only issue is that I couldn't manipulate the css. I was literally trying for 45 minutes to see what css classes were and trid chaning teh attributes but it wasnt working. So i forewent the virtual keyboard element.

**project resource links**
1. class notes:
- [Class 7 cookies integration](https://github.com/samheckle/hunter-web-design-projects-sp-26/blob/main/class-notes/cookie-session/server.js)
- [Cookies and Express Sessions](https://github.com/samheckle/web-projects-fa-25/blob/main/classes/class_13/readme.md)

2. Online resources
- https://www.w3schools.com/tags/tag_fieldset.asp
- (didn't use) virtual keyboard: https://furcan.github.io/KioskBoard/
- font website (tomorrow font) https://www.figma.com/resource-library/futuristic-fonts/
