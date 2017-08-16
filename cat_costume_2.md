---
title: Cat Costume 2
permalink: /cat_costume_2
---

# Cat Costume Project - Responsive

### Intro
Now you are going to work on making the Cat Project Responsive.

You will do this by, taking one level of the Journey into Mobile course (on CodeSchool) and then applying that level to your Cat Project.

Before you start make sure you have used git and committed the latest version of your Cat Project. You want to maintain the desktop state in case things get screwed up here.

Also add the below viewport meta element in your html's <head></head>. This is a viewport tag and keeps your browser from automatically zooming in on mobile (or smaller) devices.

```
<meta name='viewport' content='width=device-width, initial-scale=1.0, maximum-scale=1.0' />
```



#### Challenge 1: Take Level One.

[CodeSchool Journey Into Mobile](https://www.codeschool.com/courses/journey-into-mobile)



#### Challenge 2: Responsive Fonts

So we aren't actually going to use any responsive units for our fonts in the Cat Costume website... I can explain why in CG Wednesday... but basically there are 3 types of units (px, em, rem). I will explain the difference in class someday.



#### Challenge 3: Take Level Two

[CodeSchool Journey Into Mobile](https://www.codeschool.com/courses/journey-into-mobile)



#### Challenge 4: Fluid Layout

Now you should go ahead and start changing widths from fixed px units to relative percent units. This will NOT BE ALL divs or html elements. For example, you probably want the about boxes or the Get In Touch boxes to keep a certain fixed sized. But use your own discretion on what looks good. You definitely want each of the html sections to span the whole browser width.

Remember you can use both `width: 80%;` and `max-width:400px;` together. This would keep the element at 80% it's container's width, but will not ever get bigger than 400px.



#### Challenge 5: Take Level Three & Four

[CodeSchool Journey Into Mobile](https://www.codeschool.com/courses/journey-into-mobile)



#### Challenge 6: Make Your Site Responsive (Not Really Adaptive)

In today's world, we rarely make sites just adaptive. Usually we want the site to look good on ALL device and don't usually target just one particular device and screen size. This means we want our site to be RESPONSIVE.

**STEP 1: Determine widths where site breaks down**

Start resizing your screen (by dragging in the window size) from big to small. When you notice something "break", like 2 boxes sliding under each other or elements overlapping, then make note of the window width. You can see width width in the top right hand corner of your browser window but ONLY when you have developer tools opened.


**STEP 2: Add Media Query for that Break**

Now we are going to add a media query for that particular break.

Remember media queries are structured like this:

```
@media screen and (max-width: 600px){
    // styles for screen 600px and under
}
```

> hint: the max-width should be the window width you wrote down in step 1.


**STEP 3: Fix styling of the Break**

The mobile design might help you out here a little, but if spots break down before the mobile design should kick in... you should determine a good solution on your own to keep the design looking good.

Anyways, inside the media query is where you want to fix the styles that break.

For example, if you wanted to something to appear side by side like this:

X X

when the browser is greater than 700px BUT then display top and bottom like this:

X  
X

when the browser is less than 700px in width... Your code would look like this:

```
.box {
    width: 300px;
    display: inline-block;
}

@media screen and (max-width: 700px) {
    .box {
        width: 90%;
        display: block;
    }
}
```

Now go ahead and fix the css you need to inside the media query you wrote in the previous step.


**STEP 4: Repeat for all Breaks in Your site**

Repeat this process for all your sections. Keep incrementally resizing your browser to find breaks, add media queries and styles to fix those breaks. When you are done, your site should look good on ALL browsers and devices.



#### Challenge 8: Take Level 5

[CodeSchool Journey Into Mobile](https://www.codeschool.com/courses/journey-into-mobile)



#### Challenge 9: Ehh, not that Important

Most of the last level isn't important for you now, like changing out 1x to 2x images. If you haven't already, fix the splash (batman cat) image and the maps image to be fluid and respond to the width of the browser.


MOST IMPORTANTLY! COMMIT ALL YOUR GOOD RESPONSIVE CHANGES WITH GIT SO YOU DON'T LOSE THAT STUFF! That is all. Great Work.



#### Still Confused? Or just want a Debrief of What you Learned?

Here is a nice reading with pretty images to debrief all this stuff you just did! The person who wrote it is focusing on styles changing from desktop to tablet to mobile. It would be good to skim and look at the pictures. You might pick up some tips for the next project you create :)

[Responsive Design Article](https://internetingishard.com/html-and-css/responsive-design/)
