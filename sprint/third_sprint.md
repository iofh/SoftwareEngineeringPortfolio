---
layout: page
title: Sprint
permalink: /sprint/third_sprint
---

# Third Sprint

## Professional achievement
---

#### Managing team

I have more experience in programming. So i am tasked to divide our sprint backlog task to each members. After the second sprint i notice that Frederic could not take on a more technical task. Therefore, in this sprint i decided to give him a designing task. 

My task would be creating a create/delete/update scores and his task would be making the score list look good. 

    "The best architectures, requirements, and designs emerge from self-organizing teams." 

Frederic will take on a task that he is comfotable with and instead of having to get stuck on coding something for the whole sprint and not achieving anything. 

Individuals who are good at something should do the things they are good at to maximize efficiency.

#### Time management

As we plan for our sprint. I suggest that we should do only the essential task for this sprint as every person in our team has assignment on other papers due in the following weeks. We are still keeping the ammount of work. And we will still delivery what the client wants. The only part that we are not doing is creating extra feature for the client to review. This is because if the client does not want the extra feature, we will need to satisfy the client and discard the feature. That means all the time spent on the feature will be wasted. 

#### Ethical Consideration

I added the email verification function. This is because if a person could create multiple accounts to submit unlegitimate score. With the email verification. The user is forced to use a valid email. Creating multiple account would be a hassle, this will reduce the number of unactive account.

#### Communication with teammates

In order to add the email verification, our .env needed to include the password for the smtp account. I communicated with my teammates and tell them that they needed to edit their .env file for the smtp to work.

![Communication](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/thirdSprint/emailVerify.PNG)


## Technical achievement
---

#### Create/Update/Delete Score

I took on the task of creating the controller for create/update/delete score

[Commits for the Create Score](https://github.com/SoftEnOP/op-stats-sw602/commits/Create-Scores)


I added a drop down list for the games available 

![Drop Down List For Games](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/thirdSprint/dropDownList.png)

I also used the Auth::id() method to get the user id of the user who created the score and store it in the database along with the score.

![Getting User ID](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/thirdSprint/gettingUserID.PNG)

#### Adding middleware

Following what the client wants, I made it so that other non-register and non-login user cant access the Add Games and Add Scores function. Only registered accounts can add games and scores. 

The code to stop unauthorized access to certain method in the controller.
![Middleware to stop unauthorized access](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/thirdSprint/middleware.PNG)

#### Adding email-verification

Only verified email can access the add games function 

![Verify Email](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/thirdSprint/VerifyEmail.PNG)

I created an account that sends our email for every user when the register an account on the website. 


This is the [tutorial](https://www.itsolutionstuff.com/post/laravel-58-email-verification-exampleexample.html) that helped me with the email verification function 