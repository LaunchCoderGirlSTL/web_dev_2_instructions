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

Our goal: To use our new knowledge to implement a prompt that asks the user to enter a student's expected college graduation date and then based on the entered month and year, welcome the high school or college student.

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

It should take 2 parameters a gradDate (like "May 2018") and a welcome function. This function should use the grad date to figure out what graduating class the student is in (like Freshman, Sophomore, etc), then call the welcome function and pass the correct graduating class as a parameter.


**STEP 4: Prompting User**

We need to prompt the user twice. One time for the student's college graduation year and one for the student's college graduation month.

> To simplify things we are going to assume that there are only 2 possible graduation months... May and December.


**STEP 5: Processing User Prompt**

If the user input was not empty...

use the college grad year to figure out if the student is currently in high school or college...

then call the welcomeStudentByGraduatingClass, sending it the gradDate and the correct welcome function you want it to use.


**STEP 6: Test If It Works**
```
User Input Month: May
User Input Year: 2018
Output: "Welcome Senior!"

User Input Month: May
User Input Year: 2023
Output: "You're still a Junior in high school!"
```

**STEP 7: Bonus Challenge**

What happens if the user enters a college graduation date of 2026 or higher?

Currently we don't have a case to handle that in our code. So create one! You can create a new welcome function and the correct logic to your other code to correct have the following input output.

```
User Input Month: May
User Input Year: 2028
Output: "whoa, college is some years away..."
```

#### Level 2 & 3: Closures and Hoisting

These levels are definitely abstract. In practice, you don't spend a lot of time thinking about these things. So for these levels, just watch the videos and complete the challenges. There is nothing really to "practice" here. Since these are really complex examples and a lot of frameworks have their own way of dealing with these things.

[CodeSchool - Javascript RoadTrip 3 - Level 2 & 3](https://www.codeschool.com/courses/javascript-road-trip-part-3)

Now we are ready to move onto Objects... some more practical stuff.



#### Level 4: Objects


**STEP 1: Complete JS 3 - Level 4**

[CodeSchool - Javascript RoadTrip 3 - Level 4](https://www.codeschool.com/courses/javascript-road-trip-part-3)


**STEP 2: Creating Your First Object: the Teacher Object**

Slowly but surely we are going to change our teacher, student and course variables into objects... but let's start with the teacher.

Take a moment before we start... look at the variables we currently have for a teacher, and write down a list of possible property names we might give a teacher object.

Okay cool! Got the list? Does it match mine?

```
name
department
ratings
addRating
getAvgRating
```

Let's start with the list and create a teacher object... with just an object literal declaration (with the curly brackets)...
```
var teacher = {
    // list and fill properties here
};
```

1) create the properties name, department and ratings and fill them with the correct values.

2) still have the addRating function? let's move it from outside the teacher object to inside the teacher object. To do that you will have to make it an anonymous function (remove function name), because the property addRating will now be the "name" of the function.

There is something else we can do as well. Since we will only want to add to the ratings array that is the property of the teacher object, we can remove the ratings parameter and use that special word `this` to access the teacher's object ratings array... make sure to keep the newRating parameter. That will still have to come from "outside" the object.... stuck on this one? here is a little bit of help...

```
var teacher = {
    // pretend there are other properties here
    ratings: [3.5, 1.0, 5.0],
    addRating: function (newRating){
        this.ratings.push(newRating);
    },
};
```

you also don't need to return the new array, bc it will add it to it's own object. Okay let's move on to the getAvgRating function.

3) Move the getAvgRating function to the teacher object. Remember if any thing inside the function references a property of the teacher object, you should use the `this` keyword to access that property.



**STEP 3: Using Your Teacher Object**

Remember those prompts you created for your teacher object... well we are going to reuse those, but instead of using our old teacher variables, we are now going to use our new teacher object to make sure everything is working correctly.

To do this you will need to change the addTeacherRating call. You now need to call your addRating property on your teacher object and only pass in the userRating.

Also test to make sure the addRating function is still working, along with the getAvgRating function by printing out the avg rating before and after you add the new rating.

:)


**STEP 4: Create A Course Object**

Create a course object with the following properties.

```
name
department
teacher
semester
```

Now it's time to change out that double array we currently have. Remember that courses array that hold course as arrays. Well now we have a course object.

Change out the course arrays with object that have the same properties (but different values) as the course object you created above.


**STEP 5: Fix the filterCourses function**

Oh no. This might have broken your filterCourses function. Let's update it so it works again.

We used to access the course department with `course[1]` ... how do we change that to get the department property of a course object?

Go ahead and try to update the filterCourses function and text it with the user prompt you created earlier. :)


**STEP 6: Adding an object as a property of another object**

In our course object we have teacher property. Currently that teacher property is just a string. But wouldn't it be cool if it was actually a teacher OBJECT! That was we could access the teachers name, department or even avg rating.

Change out the string teacher value in the course object for an actually teacher object. You can create a new object with the same properties as the teacher object OR use the teacher object variable you created in step 1.

Now to test that this worked, let's test this. Console log a course's teacher name.

Hint: you might have to use the dot operator a couple of times. :)



Okay that is enough for now. Let's move on to learn about Object Prototypes before we continue editing this js file.



#### Level 5: Prototypes

**STEP 1: Complete JS 3 - Level 5**

[CodeSchool - Javascript RoadTrip 3 - Level 5](https://www.codeschool.com/courses/javascript-road-trip-part-3)


**STEP 2: Turn the Teacher Object into an Re-usable Object Prototype**

Currently your teacher object should look something like this:
```
var teacher = {
  name: "Sally Smith",
  department: "Physics",
  ratings: [4.3, 5.0, 4.7],

  addTeacherRating: function(newRating) {
    this.ratings.push(newRating);
  },

  getRatingAvg: function() {
    var total = 0;
    for(i=0; i < this.ratings.length; i++) {
      total = total + this.ratings[i];
    }
  return total / this.ratings.length;
  }
};
```

Great! Our code is looking a bit more organized than when we had all those variables individually storing everything. But there is one more improvement we can make... Re-usability! With our current teacher object, we would have to re-make the object literal with every new teacher like:
```
var teacherSally = {
  name: "Sally Smith",
  department: "Physics",
  ratings: [4.3, 5.0, 4.7],

  addTeacherRating: function(newRating) {
    this.ratings.push(newRating);
  },

  getRatingAvg: function() {
    var total = 0;
    for(i=0; i < this.ratings.length; i++) {
      total = total + this.ratings[i];
    }
  return total / this.ratings.length;
  }
};

var teacherBobby = {
  name: "Bobby Smith",
  department: "Physics",
  ratings: [4.3, 5.0, 4.7],

  addTeacherRating: function(newRating) {
    this.ratings.push(newRating);
  },

  getRatingAvg: function() {
    var total = 0;
    for(i=0; i < this.ratings.length; i++) {
      total = total + this.ratings[i];
    }
  return total / this.ratings.length;
  }
};
```

Not the best. We did all that work with our functions and now we can't even re-use the function. So solve this problem we can turn the teacher into an Object Prototype (or class).

First, create a Teacher constructor. Remember Javascript Constructors are just functions that names are capitalized.

```
function Teacher (<parameters go in here>){
    // set initial values in here...
}
```

This constructor should take parameters to give the Teacher properties their initial values. So for the Teacher class, we need parameters for name, department, and maybe ratings (if you want to, we could also just add their ratings later with the addTeacherRating function, so up to you). Then inside the Teacher Constructor function you need to set the teacher's properties using this... like:
```
this.name = <whatever you named this parameter>;
```
You should have code like this in your constructor for whatever properties the teacher class has ... in this case... name, department and ratings... all need to be initialized to some value.

Not done yet! what about the functions. Where do we add those?!? Well since those are properties of the teacher object but do NOT need to be "initialized" or set to default values... we can add them to the teacher object AFTER the constructor with:
```
Teacher.prototype = {
    // define other properties in here
}
```

So now add the addTeacherRating property and the getRatingAvg property to the Teacher.prototype section.

YEAH your Teacher Prototype should be done!

**STEP 3: Create new Teacher Instances**

Now it's time to make use of the Teacher object re-usability!

Let's create 3 new teachers, using the new key word like:
```
// remember to pass in parameters that your construtor takes
var teacherSally = new Teacher("Sally Smith", "Phsyics", [5.0, 4.3, 4.1]);

// repeat 3 times with different parameters to create different teachers...
```

now we can add ratings to each of those teachers, get their avg ratings and print them out to make sure everything is working...

Print out the below information to the console... do this with each teacher!

```
Sally Smith
Physics
Avg. Rating: 4.6
Adding Rating: 5.0
New Avg Rating: 4.7
```

Wow! Javascript Prototypes are cool!

**STEP 4: Create Course Prototype**

I am not going to give you so much instruction on this one, but to make the Course variables a prototype follow the same method as we used for teachers...

1) Make a constructor
2) Create new instances of the Course Class to fill your courses array.

Note: You may have to adjust your filterCourse function... just I would test to make sure it still works. :)

But wait, what should the teacher property's value be? A teacher's name?
Well now that we have a Teacher Class and new teacher instances, we can use a teacher instance instead of just a teacher name. In the Course constructor, we can pass it a teacher instance to assign the teacher property.


**STEP 5: Create A Student Prototype**

It's been a little bit since we have touched the student section of this JS file. So let's go ahead and create a Student Prototype as well... The student prototype will need the properties name, major, email, avgGPA, and a courses array.

After you have created the Student class constructor. Let's add some additional functionality to the student class. Add the following...

addCourse - function - takes a course parameters, and adds it to the Student's courses array.  
dropCourse - function - takes a course parameter and finds it in the course array and removes it.  
changeMajor - function takes a string parameter and changes the Student's major property

yeah! We should be done with the Student Prototype! Now let's create some instances of that Prototype.


**STEP 6: Using the Student Prototype**

In your html/css that you made, create a new variable for each student you have listed in your design... and store a new instance of the Student Object. Making sure to pass in all the parameters that the Student constructor needs.

Then test the new functions you added!
Pick one student and a course... and use the addCourse property to add that course to the student's courses array... then let's console log some things to make sure it is working correctly...

```
Adding Course: <course name>
To Student's Courses: <student name>
Now they are taking....
<list course names of all courses the student is taking>
```


**STEP 7: Conclusion**

WAY TO GO!! ALL OF OUR CHAOTIC VARIABLES ARE OBJECTS AND REUSABLE! THIS IS AMAZING!


Now, let's clean up your code and make sure it is organized and properly spaced... maybe add some comments in places where you figured out something confusing.. the USE GIT AND COMMIT!

Onto jQuery ... then we will use these objects to populate our different pages :) YEAH!
