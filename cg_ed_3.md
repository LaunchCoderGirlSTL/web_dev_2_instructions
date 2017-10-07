---
title: CG Education - JS 3
permalink: /cg_ed_3
---

# CG Education - Javascript Part III

### Intro
With the other CG Education challenges, you first went through the whole JS course and then completed the challenges. However, the 3rd course is a lot to take in. Some is more important than others, so we are going to break it down a bit.


To start, go ahead and open your terminal, navigate to that project, and make sure all your work from the last CG Education JS Practice is committed with git. Now open the project directory with your text editor and let's begin!



#### Level 1: More About Functions

Before you start Javascript RoadTrip 3, there are some things to note...

There are some extremely convolute examples in this level. Very rarely will you have javascript that is written in such a manner, but nonetheless CodeSchool is trying to push the boundaries of javascript and increase your logic skills. So my advice...

Try to take in what they are saying and complete the challenges, but if you are feeling confused and not exactly clear on the whole thing... no worries. I will help you practice the important parts of the level.


**STEP 1: Complete JS 3 - Level 1**

[CodeSchool - Javascript RoadTrip 3 - Level 1](https://www.codeschool.com/courses/javascript-road-trip-part-3)


Now let's go back to your cg education project.

Our goal: To use our new knowledge to implement a prompt that asks the user to enter a student's expected college graduation date and then based on the entered month and year welcomes the high school or college student.

**STEP 2: Welcoming Some Students**
Now we are going to practice writing some anonymous functions. Yay!

Write 2 anonymous functions and store then in variables called... welcomeCollegeStudent and welcomeHsStudent. Each will take one parameter, the student's class (like Freshman, Sophomore... etc).

The college welcome function should alert the following message...
```
"Welcome <students-class>!"
```

The high school welcome function should alert the following message...
```
"You're still a <students-class> in high school!"
```

Write one more function called gradDate (this can be anonymous or just a function expression). It should take 2 parameters a month and year and return the two put together. For example...   
inputs: `May` and `2018`  
outputs: `"May 2018"`  


**STEP 3: Using welcome functions as parameters**

Now let's create a function called welcomeStudentsByGraduatingClass.

It should take 2 parameters a gradDate and a welcome function. This function should use the grad date to figure out what graduating class the student is in (like Freshman, Sophomore, etc), then call the welcome function and pass the correct graduating class as a parameter.


**STEP 4: Prompting User**

We need to prompt the user twice. One time for the student's graduation year and one for the student's graduation month.

> To simplify things we are going to assume that there are only 2 possible graduation months... May and December.


**STEP 5: Processing User Prompt**

if the user input was not empty...

use the college grad year to figure out if the student is currently in high school or college...

then call the welcomeStudentByGraduatingClass sending it the gradDate and the correct welcome function you want it to use.



#### Level 2 & 3: Closures and Hoisting

These levels are definitely abstract. In practice, you don't spend a lot of time thinking about these things. So for these levels, just watch the videos and complete the challenges. There is nothing really to "practice" here. Since these are really complex examples and a lot of frameworks have their own way of dealing with these things.

[CodeSchool - Javascript RoadTrip 3 - Level 2 & 3](https://www.codeschool.com/courses/javascript-road-trip-part-3)

Now we are ready to move onto Objects... some more practical stuff.



#### Level 4: Objects


**STEP 1: Complete JS 3 - Level 4**

[CodeSchool - Javascript RoadTrip 3 - Level 4](https://www.codeschool.com/courses/javascript-road-trip-part-3)


**STEP 2: Creating Objects**

TBD: More to Come...
