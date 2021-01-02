---
layout: page
title: Sprint
permalink: /sprint/pre-sprint
---

# Pre-Sprint


Before our first sprint. Our team had to learn how to set up laravel.

### 5/08/2019
We were given a [tutorial](https://morioh.com/p/9b8c8ef67bd5/laravel-5-8-tutorial-from-scratch-for-beginners) to help up set up our laravel website. 

In the tutorial, some of the instruction is vague and hard to follow. 

First encountered problem:

    >Let’s create navbar.blade.php in inc folder and add the markup

The instruction does not specifically say to create an inc folder. Therefore, i kept finding the inc folder. After a few minute of seraching, i got help from Martin and Elise. Which is to create a inc folder by myself then put the "navbar.blade.php" in the inc folder.

Second Problem:
After running "php artisan serve", i got this problem.
 >RuntimeException No application encryption key has been specified.

Most of the student in the class does not appear to have this problem. I am the only one with this problem. I had asked Martin for some help. However, he had also never seen this problem. 

With some googling. I found a [solution](https://stackoverflow.com/questions/44839648/no-application-encryption-key-has-been-specified) on StackOverflow. To fix the problem. All you need is to enter "php artisan key:generate" to generate a key and "cache php artisan config:cache" to clear the cache.

### 6/08/2019
Continue working on laravel outside of class. I manage to finish the whole tutorial. Unfortunately, the website still does not work. It showed another error  

![laravel class not found error](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/class_not_found_error.png)

    > Class 'App\HTTP\Controllers\Todo' not found

The solution i found for this is found [here](https://laracasts.com/discuss/channels/laravel/fatal-error-class-apphttpcontrollerstask-not-found ). "use App\Task;" is needed on the top of the TodosController.php file.

### Final Result
![Todo list](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/todo.png)

![Todo list](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/todo2.png)

![Todo list](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/todo4.png)

![Todo list](https://softenop.github.io/individual-portfolio-19-2-iofh/photo/todo3.png)