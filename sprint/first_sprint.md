---
layout: page
title: Sprint
permalink: /sprint/first_sprint
---

# First Sprint

On 15th August, i took the initiative to get the Laravel Framework set up on our team github repository. 

Knowing that i am still unfamiliar with laravel and the Model–View–Controller(MVC) architectural pattern. I decided to start early and if any problem occurs, there will still be time to seek help from the lecturer or my teammates.

__First Sprint User Stories:__
![First Sprint - User Stories](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/firstSprint/firstSprintUS.png)



## Professional achievement
---

### Ethical considerations.

Laravel framework automatically provide the method to read and write from a database. It also hashes the password and stores the hashed password in the database.

__Hashed Password in database:__
![Hashed Password in database](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/firstSprint/hashedPasswordInDB.png)

I did not remove or change the hashing method to make the user's password appear as plaintext password. 

__Laravel Hashing method:__
![Laravel Hashing method](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/firstSprint/hashingMethod.png)

__Changing the hash method to show the password in plain text is unethical__.

Although i did not do anything coding to show that i have ethical  consideration, i did some [research](https://laravel.com/docs/5.0/hashing) to make sure that laravel does hash its password by default. I wanted to protect the user's credentials and therefore this might be an evidence that i do have some ethical consideration.
Laravel uses bcrypt for its hashing algorithm and there's a library for Argon as well if we wanted to use Argon. 

### Teamwork

After understanding all of the laravel tutorial on making a Todo. I decided to call a meeting for our team to redivide our individual task. Previously, we decided to divide the our task by user stories. But that method is not efficient and is messy. Following the agile principle "The best architectures, requirements, and designs emerge from self-organizing teams.". I understand that our method is not good enough therefore i call for a change on how we devide our task.

After discussing, we all agreed on creating the base file first. By using "php artisan make:model Game -m" & "php artisan make:controller GamesController" to let the framework create the base file, then we divide our task by letting one person do the View Game, one do the Create Game, One do the Edit/Delete Game. 

By creating those base files, we will not run into many merge conflict and the task are split more evenly.

On 21/08/2019 class time, since i had already did the login/register task. I took on the role of looking over our project code. I wanted to make sure all our code matches up and will generate a working webpage. Instead of having non functional website. Therefore, I look over my teammates' code and gave assistance on their tasks.

On 23/08/2019 Dales day, Sen is having trouble with his individual task. Since i am with him at that time, i provided assistant with his individual task and completed it. His task was to create the view and controller method for "View Games". The [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/061ffd84b21fd67fff5f2a179691cf13d067b4e8) that i help Sen with.

These evidence showed that i am a team person, i willingly help others on their individual task. As i wanted our team and our project to succeed.

### Communication With Client

We communicate with our client to set up a meeting to review our first sprint

![User Stories](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/agile/com_with_client1.PNG)

This shows that we want constant communication with our client and let our client review our progress every 2 week. In order to know what the customer wants and satisfy the customer needs so the customer could gain the upper hand in the industry,

## Technical achievement
---

For my technical achievement, i had worked on the Register/Login account function for our project. 

I initially thought it would be a difficult task to achieve. However, with the help of this [tutorial](https://www.youtube.com/watch?v=SbPYrndtjJ4). Everything is done in just a single command in gitbash. 

The formating on the website changes with the added login/register function. With a bit help in the tutorial video, i manage to change our project website back to its original format along with the additional function of login/registering account. 

Command to create the authentication function 
    > php artisan make:auth


Result


   ![Account Authentication](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/firstSprint/authentication1.png)


   ![Account Authentication](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/firstSprint/authentication2.png)
 
 
   ![Account Authentication](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/firstSprint/authentication3.png)


[Commits](https://github.com/SoftEnOP/op-stats-sw602/commit/3d8ff0a370e0f344cf8741e70870e7c770c6faac) of my technical achievement