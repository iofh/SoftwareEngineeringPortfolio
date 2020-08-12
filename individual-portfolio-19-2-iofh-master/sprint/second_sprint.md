---
layout: page
title: Sprint
permalink: /sprint/second_sprint
---

# Second Sprint


## Professional achievement
---

### Teamwork

On the day of our meeting with the client. I noticed that Frederic had not finished his task. In order to show the client a working website. I helped guide Frederic in finishing his task. This [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/f4a04f4ed7fa2121f814afdb4d0d1e5c38725016) shows all the code i helped him to produce. 


### Agile techniques

#### Working software is the primary measure of progress.

From what i mention in the Teamwork area, i noticed that Frederic had not finished his task. I could just leave him be and show the customer an unfinished product. However, as an agile software developer. I spend my time to help Frederic finish his task so that our client can use a working website. 

#### Our highest priority is to satisfy the customer through early and continuous delivery of valuable software. 
If i did not help out Frederic with his task. We would not be able to satisfy our customer through early and continuous delivery of valuable software.

Therefore, me helping Frederic with his task shows that i am being agile.

#### Scrum master

I took on the role of scrum master for the first and second sprint. This is because i have more experience in programming and i understand how the task should be divided. 
![Dividing Up Task](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/personal_reflection/second_sprint_divi_task.PNG)



## Technical achievement
---

#### Search Function
I created the search function for the game controller.

    public function search(Request $request){
        $search = $request->get('search');
        $games = DB::table('games')->where
        ('title','like','%'.$search.'%')->paginate(5);
        return view('games.search',['games'=>$games]);
    }

The code above sits in the games controller. It passes the filtered games to the view and showed the games the user searched.

The [link](https://laravel.com/docs/5.8/queries) to the Laravel documentation that helped me achieve the search function. The [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/738a47be4533a3fb61aee833c7de4a11bf249377) to the search function.

#### Referencing data from and to another table

I also clean up some of Frederic's code that i help him with. This [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/526a671ce014cd55d9c7735203c1f74e448d5d4a)  shows the things done to the show score area. I passed in the required table in the database from the controller to the view and show the data in the view.

I made the user_id, game_id in the score table reference its table. Instead of showing the user_id and game_id, i made it show the username and game name.

The database only had the id of the game and user. I passed in the user and game table to make the id of the game reference its name.

Score table with just game and user id
![scoreTable](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/secondSprint/scoreTable.PNG)


This blade template shows the code that makes the id reference the right name
![scoreReferencing](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/secondSprint/scoreReferencing.PNG)


#### Cleaning up the search view

I edited the html to make the search button sit beside the search bar instead of having it sits down below the search bar.

From this:
![Search Button Down](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/secondSprint/SearchButtonDown.PNG)

To this:
![Search Button Up](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/secondSprint/SearchButtonUp.PNG)