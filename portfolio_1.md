---
title: Portfolio 1
permalink: /portfolio_1
---

# Setting Up Your Portfolio Project

### Intro
Time to start writing some code!

You are going to start your Programmer Portfolio. This is what programmers typically use for their "resumes". It will hold links to all future projects as well as information about you!

We will start developing it here in the Learning Track but the real work on it will be done in the Project Track. For now, we are using it to practice writing code.


#### Challenge 1: Create your HTML and CSS file.

**STEP 1** Create a new directory in your home directory to keep all your coding projects (I would probably call it "Projects" or "CoderGirl" but whatever works for you!).

**STEP 2** Create a new directory IN that directory you just created for your project files. Recommend Name: "portfolio_project"

**STEP 3** Open your project directory in Atom (the application you should already have downloaded).

**STEP 4** Create File Structure (you should be able to do within Atom).

- create html file... index.html
- create styles folder
- create images folder
- create css file main.css IN your styles folder

Your file structure should look like this:
```
portfolio_project/
    images/
        (empty for now)

    styles/
        main.css

    index.html
```

**STEP 5** Copy and paste your starting HTML and CSS.  

_note: this is common practice in web development, starting with some html shell code._


HTML
```

<!DOCTYPE html>
<html>
  <head>
    <title>Your Name</title>
    <link rel="stylesheet" type="text/css" href="styles/main.css">
    <meta content="width=device-width,maximum-scale=1.0,initial-scale=1.0,minimum-scale=1.0,user-scalable=yes" name="viewport">
  </head>

  <body>
    <div class='header'>
      <h1>Your Name</h1>
      <h2>Your Tagline</h2>
    </div>

    <div class='content'>
      <img src="images/thumbnail.png" alt="Your Github Username" class="thumbnail">
      <p>
        Who are you? What are you interested in? What are you doing to learn to code?
      </p>
    </div>
  </body>
</html>

```

CSS
```
body {
  background-color: #eeeeee;
  color: #030303;
  margin: 0;
  padding: 0;
}

.header {
  padding: 15px;
}

.content {
  background-color: #030303;
  color: #eeeeee;
  padding: 15px;
}

p {
  margin: 0 15px;
}
```

#### Challenge 2: Update the HTML

**STEP 1** Update All Text, including your name, tagline and a little description of yourself.

**STEP 2** Replace the Thumbnail Picture, with a picture of yourself.

**STEP 3** Change the colors of the site to match your preferences :)

That’s it for now! You will be coming back to this project to keep practicing what you have been learning.
