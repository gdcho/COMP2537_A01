# COMP 2537 Web Development 2 Assignment 1
For this assignment you will be creating a simple website using Node.js. You will also be creating and
connecting to a MongoDB database to store the users with their names, emails and passwords. You will
create a publicly accessible MongoDB database using Atlas (at: https://www.mongodb.com/atlas).

If a user successfully authenticates (provides the valid email and password) a session will be created to
store the user's information. A user is considered logged in if they have a valid session. You will store the
encrypted session information in a MongoDB session database. A session should expire after 1 hour. If
a user is not logged in (doesn't have a valid session) they should not be able to view the members page –
it is a member's only page after all!

We will be taking input from the user to capture their account information and for them to log in. We'll
need to properly deal with NoSQL Injection attacks in our MongoDB database so that users can't
intentionally attack our database.

We will use a .env file to store encryption secrets and your MongoDB database credentials. Passwords
should not be stored in your git repo. If they are, and your repo goes public or accidentally gets leaked,
an attacker now has access to your database to do whatever they want with it! Let's keep our passwords
out of the reach of hackers.

Your site needs to be hosted on a site like Qoddi. Qoddi is a fully managed web app hosting platform
(https://qoddi.com/). Qoddi can provide many features including: 1) getting us off our localhost so we
can share our sites with other people; 2) creates a domain which is publicly accessible; 3) installs and
runs our node.js server; 4) automatically deploys our code when we make a commit and push our code
to our main branch on github.
