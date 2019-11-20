Directions for connecting back end and front end with expresss and node.js 

1. Clone the front end repo to your local device. Make sure you do a npm install, npm run build, and then npm start.
If you are unfamiliar with this frontenders can help you, and I can help set you up.

2. Fun with database time. Go here: https://www.ampps.com/wiki/How_to_use_AMPPS. Copy round 2 sql code into new database. Alternatively, I can put the code in a file called round2code for convinience.

3. If you have ammps, wamps, mamps, you have to look for a settings config file (for me it was the settings button next to ammps). You need to comment out the line # innodb_force_recovery = 1 by putting a hash tag in front of it. save and restart mysql.

4. Once you have sql running and database up, we are set to move forward with the node js and express code that connects us to the database.

5. Take a look at Server.js file in front end. It has most of the code related to connecting backend and front end. I watched this video to help understand what node.js is: https://www.youtube.com/watch?v=TlB_eWDSMt4&t=4179s (feel free to watch on double speed). -Also **this video mimics how I set up node.js in Server.js file of front end: https://www.youtube.com/watch?v=HPIjjFGYSJ4&t=115s&fbclid=IwAR2daqIIiajepOOvq9C46QG6UI3_acSTxpulBGbG9ifpR_oaJqNaL2KJhaI

6. To run the local server for the json, **important step, go to command prompt and enter node Server.js it should run and say 'connected!' ...test this by hitting up http://localhost:4000/lighting ..if there is something there it worked

7. Feel free to try and test grabbing info and putting info into database by reading how to in these brief tutorials from w3schools: https://www.w3schools.com/sql/sql_select.asp -You will be able to see if it worked by hitting http://localhost:4000/lighting, which should output the json for a part of the database.

8. We can grab the data, do calculations, and display it using axios (get, post) or ajax(fetch) calls. https://www.w3schools.com/xml/ajax_intro.asp (ajax) for example


Other files in this repo:
1. file with round2 slq code
2. file with screenshots of what it should look like
