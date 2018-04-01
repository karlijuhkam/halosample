This is a test for evaluating Upwork candidates.

Goal
===
Complete the user story "As an authenticated user, I want to sort the table on the Users page by clicking on the table headers" in accordance with the following:

How to set up the project
====
1. Clone the project to your computer. If you just download the zip file, you will lose the files beginning with a dot like .htaccess and .gitignore. So do not download zip. Clone!
2. Delete the <code>.git</code> folder in the project's root folder
3. Run <code>git init</code> to make a new repository
4. Copypaste config.sample.php to config.php and adjust settings there
5. Import doc/database.sql to your local mysql database
6. Run composer install
7. Install codeception globally to your computer or use vendor/bin/codecept
8. Install and run selenium server on port 4444 (or change acceptance.suite.yml to use PhpBrowser instead) 
9. Test that http://localhost/sampleproject/ opens and you can click on Users and log in with demo:demo.

How to do the story:
===
1. Create a new acceptace test: run codecept generate:cept acceptance "UsersPageTableIsSortable"
2. Write acceptance test in tests/acceptance/UsersPageTableIsSortable.php. You must get the user data from SQL (ordered by SQL query) to PHP array (you can use get_all() for that) and then compare that array with what Codeception sees on the page. If your PHP array and Codeception returned data are in the same order, test passes. Don't forget to include login steps.
3. Implement story. Put script links to master_template.php. The table is located in users_index.php
4. Run codecept run to see that the story passes
5. Commit with a message "As an authenticated user, I want to sort the table on the Users page by clicking on the table headers"

How to send me your results
===
1. Upload your project on Github or Bitbucket and send me a link to your repo along with how much would that story have cost me, if it was a real story for a real project (without taking into account the initial project setup, of course).

Pricing model explanation and how we will work
===
- I will be writing stories with the customer
- Customer decides the order of the stories
- We don't pre estimate the stories. If the customer asks, we only give a ballpark estimation. But this is just a prediction, not a commitment. 
- Then the story is done.
- *Then* we set the story time of what we think it would take us *now* to implement this story from the scratch (basically we don't take the time we spent on googling finding solutions and being on the wrong track and fixing our silly mistakes into account). 
- Then I and the customer will have a meeting where we will go over the completed stories and I walk the customer through these stories. If everything is according to story spec, I will have him accept the given story and move on to the next one with him.
- At the end of the month, we bill the customer by the cumulative hours of stories he has accepted in that month. Bugs excluded.
- The project ends when the customer runs out of either new stories or money.
- This is cost effective and a fail safe way for both parties. I expect to do business with you on the same grounds.
