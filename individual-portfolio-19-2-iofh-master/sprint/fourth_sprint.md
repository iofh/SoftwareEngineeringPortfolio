---
layout: page
title: Sprint
permalink: /sprint/fourth_sprint
---

# Fourth Sprint


## Professional achievement
---

#### Communication With Client

This sprint spans for 3 weeks. Our team originally wanted to have a meeting with our client in just 2 weeks. However, our client is away when our sprint ends. Therefore, we communicated with our client and set up a meeting when he is back in Dunedin. 

We also set a recurring meeting with our client by using the Microsoft Calender to book a recurring  meeting every 2 weeks. Our meeting with the client will be on a set date instead of having it to be uncertain every week.  

#### Teamwork

This sprint i had teamed up with Sen to make our banning/unbanning account function. In the previous sprint i did not collaborated with any of my teammates when doing a task. Collaborating helped me save some time because i do not need to do everything myself as well as improving my communication skills.

I had also helped Frederic in some of his tasks. Which is creating a group and letting user join the group. I did not help him a lot but when he got stuck i manage to guide him into the right direction. 

#### Being professional

I did some unit test on our server. Doing unit test will let me know what is happening with the code i typed in. 

[Commits for my unit test](https://github.com/SoftEnOP/op-stats-sw602/commit/2556036075b2e95655cd69ae0a7123adc0212d39)

Unit testing checks my code down to the individual method. Doing unit test gave evidence that i am double checking my code and making sure it works. I wanted my user to have a pleasant experience when using our website and not having to run into errors.

Side note: Frederic's unit test might be very similar to my unit test. [Frederic's commit](https://github.com/SoftEnOP/op-stats-sw602/commit/f35e209eb57ae9f629df225998e700d35391df34) compare to [my commit](https://github.com/SoftEnOP/op-stats-sw602/commit/2556036075b2e95655cd69ae0a7123adc0212d39). This is because i helped him with his unit test as well.

    Build projects around motivated individuals. Give them the environment and support they need, and trust them to get the job done.

I wanted to give a good environment for him to work in. Therefore, i gave him support when he need it.

## Technical achievement
---

#### Create/Update Profile

I created a profile page for each user. Logged in user can edit their profile picture and name. 
The [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/5097e0eb8a1c67e6433c29fc736ae4285499d407) to the profile functionality. 

#### Adding pictures to games

I made a function where any user could change the image of a game when they are editing  the games' detail.
The [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/95bebd1f2e7014d233e905456d848e8c7fc93194) to adding pictures to games functionality. 

With this functionality, i went into the deployment server and put in this command

     php artisan storage:link

This command is used to create a soft link to from the public/storage to the storage/app/public. So that the image could be saved on our server and can be accessed from the database. As shown in the image below.
 
 ![Picture in database](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fourth_sprint/picture.PNG)

To save the picture in the database, php needs the extension ";extension=fileinfo".
I communicated with my teammates and let them know if they wanted to save an image, they would need to include the extension.

 ![Communication With teammates](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fourth_sprint/communication.PNG)


#### Banning user

I collaborated with Sen to create this feature. A user can vote to ban a user. If a user received more than 2 votes, the user will be disabled/ban. For example, person "A" and "B" vote to ban "C", "C" will be ban. However, if either "A" or "B" lifted their vote then "C" would be unbanned. 

A user would not be able to ban the same person twice, and would not be able to ban himself.

The [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/c00096b32d148f90665ec22e307dddd03da7235c) to the logic behind the banning user

The basic concept would be person A wants to ban person B. Person A request a ban on B and the ban table will be populated with 1 vote to ban B. When another person C vote to ban B again. Another vote will be populated in the ban table. Now every ban will call a method that checks the count of the banning table. If the banning table has more than 2 votes to ban a user. The user would

#### Sorting Score/Games/User on homepage

I did not do the coding for this function. I let Sen do the task while i help with guiding him towards finishing the task. The reason of me not doing this is because i had already did some Database "order by" in the previous sprint and i wanted to give Sen the chance to do some Database filtering so he could get the marks for the project.

