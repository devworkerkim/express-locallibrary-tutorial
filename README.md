# Express Tutorial: The Local Library

This is the repo for the Local Library website tutorial from MDN as part of NodeJS course of The Odin Project.  This tutorial builds a MongoDB database for a library with NodeJS/Express as the server.

## Known Bug

There is an issue with how dates between the server and the database are treated.  Due to timezone differences between the system settings, the dates reported on the database and the dates parsed on the server will be different.

## What I Learned

### Express-Generator

I have not used [Express-Generator](https://expressjs.com/en/starter/generator.html) to create an application skeleton before.  As long as its okay to be working in the MVC \(Model-View-Controller\) design pattern, Express-Generator will set everything up so you are ready to start coding an NodeJS/Express application.  Sure beats having to create directories and figuring out how to structure them.

### Pug Template Engine

My personal preference for templating is Nunjucks, so using Pug was a challenge for me.  As with all of the templating engines, they each have their own syntax for rendering dynamic data within the HTML.  Of all the popular templating engines I researched, Nunjucks spoke to me the most because of the minimal syntax deviation from HTML syntax.

Pug, on the other hand, has been popular for a long time for its readability.  In my opinion, the indentation formating of Pug along with the lack of separators makes the syntax really hard to read.  The indentations were hard to read, especially for the code that was formatted to indent with two spaces instead of four.  Without the guidelines in my code editor, I would have been hosed trying to figure out what was nested.  There were some nesting issues encountered because of how my clipboard pasting worked in my editor.  It's an easy bug to fix, but the indentation convention leaves a lot of room for errors.

I kept using Pug in this project to try out and get some experience, but the readability was too hard for me and my preference still remains with Nunjucks.

### Async Utility Module

I'm guessing that this tutorial was written before async/await was adopted into NodeJS, but I really liked the [async](https://github.com/caolan/async) utility module.  It formats the asynchronous code in a very intuitive way, especially for those calls that need to be run in parallel.  I like when syntax semantically makes sense.