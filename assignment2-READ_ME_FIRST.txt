If you're viewing this on github.com, click 'raw' in the upper 
right corner to open the instructions full-screen.

If you get stuck on any steps, post in Slack under general.
Make sure to mention which step you are stuck on and what you've tried so far.
If you see that someone else is stuck and you know how to get them un-stuck, feel free to reply to their post(s) on slack.
							
1. Open the terminal (WINDOWS USERS: this means open git bash)
2. Complete the following tutorial:
   http://www.ee.surrey.ac.uk/Teaching/Unix/unix1.html

3. In your browser, go to the URL: 192.168.44.44
   If it says 'Welcome to VDD!' at the top of the page - you are good to continue.
   - If it does not say Welcome to VDD, enter the vdd folder through git bash, and, like we did in class, enter the command: vagrant up
   - Once this process completes, repeat step 3
   - Post on slack (under 'general') if you can't get this to work

4. In the terminal / git bash, navigate to the vdd folder we created in class.
   Execute the command: vagrant ssh
   You just connected to your server! This is where we want to get comfortable working.
   Now that you've ssh'ed in, enter (cd) the sites directory. (still in git bash / the terminal)
   Leave this window open.

5. In your browser:
   Log in to github.com.
   Go to https://github.com/debugsociety/hw , click 'Fork' in the upper right corner. (AKA "fork the repo")
   You should now have a copy of the hw directory on your github account. 

6. Go to your forked copy at https://github.com/[YOUR USERNAME]/hw
   Copy the URL on the right, under HTTPS clone URL

7. In the terminal/git bash(continuing from step 4):
   Paste and execute the command: git clone [PASTE THE COPIED URL HERE]
   A new folder should be created called 'hw'. Enter that folder (cd)

8. In that folder, execute the following (put your name where it says Your Name): git config --global user.name "Your Name"
   In that folder, execute the following (put your email where it says you@example.com): git config --global user.email you@example.com
   Git has been configured! Now your name and email will be saved with all of your commits.
   Leave this window open.

9. Windows users: download & install Notepad++
   Mac users: download & install Sublime text 2
   In the program you just installed, open the existing file: [Your Desktop]/Sites/vdd/data/hw/assignment2-editme.html
   Do the following to the file:

------------------------------------------------------------------------------------------

Step 1: Create a div, give it an ID of wrapper. This will be referred to as the wrapper div.<br />

Step 2: Create a div, give it an ID of header. This div should be inside of the wrapper div. This will be referred to as the header div.<br />

Step 3: Create a div, give it an ID of title. This div should be inside of the header div. This will be referred to as the title div.<br />

Step 4: Create a div, give it an ID of body. This div should be inside the wrapper div, but outside of the header div.

To get you started, here are the 'answers' to step 1 and 2:

Answer -> Step 1:
  <div id="wrapper"></div>

Answer -> Step 2:
  <div id="wrapper">
    <div id="header"></div>
  </div>
------------------------------------------------------------------------------------------

10. Save your file. Go back to the hw directory in git bash / the terminal. 
    Execute the command: git add .
    Don't forget the dot in the above command or it won't work. The command means 'track all files in this directory with git'
    Execute the command: git commit -m 'Homework assignment 2'

11. Type git push


Geez, that was hard! What did we just do? We practiced the basics :)

We:
- Forked a repo (made our own copy of someone else's git folder)
- Cloned the repo (made a copy from our github to our local computer)
- SSH'ed into our server (through our computer's git bash/terminal, we connected to our development server's own command line.. AKA 'our servers git bash')
- Configured our local git account globally (all of our future git commits {edits} will show the name and email you typed in)
- Used a better text editor to make a few html changes to an existing file
- Committed our changes to git
- 'Pushed' our changes up to github (uploaded our homework to github, which is publically viewable)
