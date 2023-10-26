# JeffersonCountyLibrary

## Setup
* Fork and Clone this repository
* Run `update-database`

## Exercise (12 points)

Check out a new branch and complete the following tasks **in order**:
* 2 points - There is a bug in our authentication!  Identity looks like it is set up, but we can't register users.  Find and fix this bug! (Hint: this should only take one line of code)
* 2 points - Right now, anyone can 'check out' a book.  Update the application so that only a logged in user can check out a book.
* 4 points - In this application, we have the ability to create new books.  Improve this functionality by:
  * Add a link from the nav-bar to add a book
  * Make sure only Librarians can add a book
* 2 points - Create a descriptive pull request and merge this branch into main
* 2 points - Take a screenshot of a database query result from pgAdmin that clearly shows which users in your database are librarians.  Update this README to include your screenshot below:

  ![database query result](https://github.com/SGrinstead/Launch_Mod5Week3Assessment/assets/48660896/aa400004-f61e-4c4c-bb2f-1520bba86daf)


  

## Questions (6 points)

Answer the questions below in this README.  Answer these questions as if you are in an interview!

1. What are roles and claims as they relate to Authentication and Authorization?
   Roles are something you assign a user and claims are based on information about the user. Both require the user to be authenticated already. As a real-world example, a bar checking the age of everyone entering is checking their claim of age before letting them in, and anyone with the role of employee is able to enter because the business assigned them that role previously.

3. How do cookies play a role in authentication and authorization?
   Cookies hold your session data, and in the case of auth, keep track of who you are logged in as. If you used a site with authentication and authorization without any cookies, you would have to log in every time you visited a new page, and some other features would almost certainly break. In one of my previous projects, I had multiple actions that checked who was currently logged in by using cookies. For instance, the action that updated a user's information. If I wasn't able to use cookies to do this, the app would become less secure.

5. If asked to implement Auth in a new .NET application, would you use the Identity framework?
   Identity is the Auth framework I have the most experience with, so I would use it in a new application. I used it in school to make a program with multiple roles that gave different levels of access. I had some actions only an Admin could access such as viewing message history of all users, some only a Super User could access like editing their messages, and a couple that were left open to visitors who weren't logged in to view, like a display of recent messages. I have found Identity to be easy to use, so it would be my first choice of framework to implement auth.

## Rubric

This assessment has a total of 18 points.  Earning 12 or higher is a pass!
