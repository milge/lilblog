## LilBlog

###About
LilBlog is a client-side only blog. It uses javascript, css, and html. Data is saved to a JSON file. [Check out a live demo here.](http://milge.github.io/)

###Why?
**Portability:** LilBlog will run on most current servers and has no server side dependencies. It will run on budget web hosts without any need to set up a database.

**Simplicity:** What you see is what you get. There's no difference between the files on your server and the output.

**Learning:** LilBlog is great for students learning front end web technologies without having to know server side technologies.

###Why not Jekyll/Kirby/etc?
Database-free site generators like Jekyll are great for generating sites. The downsides are having to learn a new syntax and requirements. Jekyll needs Ruby, RubyGems, an OS, NodeJS, and Python to run. LilBlog just needs server software like Apache or IIS to run.

###Adding a Post
Adding a new post is simple. Just add a new line to the data.json file under posts with the following format:

{"title": "Post title goes here", "date": "Date here", "text": "Post text or html goes here"}

###Warning: HTML in JSON
HTML doesn't always play nice in JSON strings. [There are a few things that need to be done to prepare HTML to be saved to JSON.](http://www.thorntech.com/2012/07/4-things-you-must-do-when-putting-html-in-json/)

If you have a HTML post that needs to be added, write out your post in HTML. [Then use this tool to convert your HTML to a JSON-safe string.](https://milge.github.io/html2jsons.html) The generated output will work in JSON.

###TODO:
Break out json file into chunks for performance for larger sites.

Refactor jquery functionality into native javascript.
