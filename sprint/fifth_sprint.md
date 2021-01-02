---
layout: page
title: Sprint
permalink: /sprint/fifth_sprint
---

# Fifth Sprint


## Professional achievement
---

#### Agile Techniques

After loading our newest version of our website to the deployment server. I did some testing and noticed that our website has an error for every page. The error is about the permission to read a file is denied in the mariadb server. 

I found out that it is because the mariadb server messed up the owner of some of the folder by using the knowledge i learnt in Linux. The www-data is supposed to be the owner but some files have se19s2_03 as the owner. Which means the Apache webserver does not have the permission to read the file. That is why there is an error on our website.

To fix this, i asked Rob and Martin to help me change the permission so that the error will not happen again. As far as i know, only Rob and Martin has permission for the mariadb server. 

This showed that i am an agile person. I wanted to let the customer have a working website at all times. 

    Working software is the primary measure of progress.


#### Ethical Consideration

I also noticed that our database password and our SMTP email password is shown in the laravel error. I wanted to find a solution as quick as possible. Therefore, i went to see Elise to see whether she could help with the problem. And as i quickly email Martin for help and ask Rob for help as well. 

Instead of pushing the work to tomorrow. I have ethical consideration that the user's email might be leak to the internet. Therefore, i immediately  try to fix it instead of procrastinating.

Screenshot Shown below is the evidence that i asked Rob and Martin for help imediately, after finding our the password leak.

![AskingForHelp](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/AskingForHelp.PNG)
![AskingForHelp2](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/AskingForHelp2.PNG)
![AskingForHelp3](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/AskingForHelp3.PNG)
![AskingForHelp4](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/AskingForHelp4.PNG)


#### Teamwork

I helped Frederic with his task that he did not finish in the previous sprint. Which is the join group functionality. I help him with the controller side of his task. The [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/2d830d1cc8cd8b9ef3fa5bc4d814219e858688ec) that i helped him. After that, i also improve on the controller that makes the user able to join and leave the group with a click of a button. The [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/940f8b6d0d817e4bac8a828a4496268311219a62) that shows i improve on the group's controller code.




## Technical achievement
---

#### Removing bug where if user delete games with scores in it, it will show a foreign key constrain

I remove the button to delete the games if there is a score linked to it. This is to mitigate the foreign key constraint error from happening. I also use the same function for the group. Where if there are users in group. You could not delete the group. The [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/fdf8a306f747ffeb6dae7598ecea1b5091518888) to the functionality. It is done in the view. It checks for whether the score(array) is empty. If so then allow the delete modal to appear.

![deleteWithScore](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/delete_withScores.PNG)

![deleteWithoutScore](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/delete_withoutScores.PNG)


#### Fix some formatting

I fix some formatting on our website to make sure it looks good. I added some dropdown list on the navbar. Instead of having ViewGroup AddGroup. I make it a drop down list where it only shows Group and after you click group it will show ViewGroup and AddGroup

![DropDown](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/DropDown.PNG)

With the new format. The user will have a better time navigating through our website without having too much information on their screen.

#### Fix Score not sorted properly

Sen told me that the score is not sorted properly on our website. I found out that our score datatype is VARCHAR and it is sorted differently from integer. This [Website](https://www.copterlabs.com/natural-sorting-in-mysql/) shows the problem we had in when sorting the score. 

Before changing it from VARCHAR

![Sorting](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/sorting.PNG)

After changing it to INT

![Sorting2](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/sorting2.PNG)

I created a new migration script using the command from laravel to make the migration script

    > php artisan make:migration 

The picture below shows the code i put in the migration script. ![Migration](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/MigrationScript.PNG)


#### Adding Join group and leave group functionality

As i said in my professional achievement. I created a join and leave group button so that the user could not just keep joining the group. The picture below shows the functionality. This is the [commit](https://github.com/SoftEnOP/op-stats-sw602/commit/940f8b6d0d817e4bac8a828a4496268311219a62) for the function


When Joining the group

![joingroup](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/joingroup.PNG)

Feedback when joining the group

![joingroupfeedback](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/joingroupfeedback.PNG)

After you join the group

![groupjoined](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/groupjoined.PNG)

Feedback after leaving the group 

![leavegroupfeedback](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/fifth_sprint/leavegroupfeedback.PNG)
