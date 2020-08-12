---
layout: page
title: Sprint Reflection
permalink: /personal_reflection/second_sprint_ref/
---

# Second Sprint

## What went well

I managed to get the search function working, showing scores on a game. 

We also managed to deploy our first working website to the internet. Which is agile because we delivered working software to our client in just 2 weeks. 

Although there are still many functions that are yet to be done. The essential function of creating an account, making a game and showing a game is deployed on the website. 

I had also learnt more on the MVC and Laravel framework. 

I also used scrum framwork(stand up meeting) to know my teammates progress in our sprint.

## What needs to be improved

Firstly, we did not have enough time for our sprint. We did our meeting with our client on 28/08/2019 and our end of sprint is on the 6/09/2019. Which meant that we only have about 9 days to finish our sprint. And we agreed on too much task giving by the client. 

##### Communication with my teammates

I took on the role of dividing our second sprint backlog for my teammates. 
![Dividing Up Task](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/personal_reflection/second_sprint_divi_task.PNG)
However, i did not explain well enough for Sen and Frederic on what they need to do exactly. I just told them to work on the migration of creating  a score and connect the user id and the game id to the score. 

Nearing the end of the sprint i found out that they did not clearly understand what their task is. I should have communicated more with them.

Thankfully, i managed to help Frederic with his task. And we managed to finish our sprint and present it to our client.


#### Taking/agreeing on too much task in a short sprint

I assume that the search function would be a command in laravel, which is not the fact. I spend the rest of the few days trying to work out the search. I only got it working nearing the end of the sprint.

While i was busy with my own task. I was unable to help my teammates. Only after i finish my task then i am able to help them. 

Therefore, i think that we should take less task for the next sprint so that i could help my teammates.

## What lesson did i learn

#### MVC

I learnt more on laravel blade template and more on the MVC. I understand how to pass in data from the database from the controller to the view. And i know how to use routes to connect all the views together. I am also more fluent and comfortable in using the blade template.

#### Time Management

Due to our late start in our sprint, i learnt how to manage my time and also i learnt how to prioritize my time. For example, i started early on doing the search function just in case i get stuck and not know how to do it for a week. Which i did. Thankfully i started early or else i wouldn't be able to provide the search function for the customer.



## What barriers did i encounter

#### Unfamiliar with laravel
I did not understand how to pass in data and how to filter data for my search function. Therefore, i spend few days stuck on trying to look at tutorials online which only [one](https://medium.com/justlaravel/search-functionality-in-laravel-a2527282150b) of them help. However, i only copied the HTML form. The tutorial uses the route to control the data which is not what i want. I wanted the controller to be the one who controls the data.  

After taking my time to go through the laravel database documentation i manage to know how to use the [WHERE](https://laravel.com/docs/5.8/database) function to filter data and i finally know how to pass in data from the controller to the view.

        $games = DB::table('games')->where('title','like','%'.$search.'%')->paginate(5);
        return view('games.search',['games'=>$games]); //passing in the games database to the view


Other than being unfamiliar with laravel, not much is barriers was encountered.
