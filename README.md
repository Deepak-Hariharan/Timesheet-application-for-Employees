Integrated Timesheet for OAG
Author:
Deepak Hariharan B00928025
Yutong Yang B00932249
1. INTRODUCTORY INFORMATION
Client
node_modules: contains all the dependent packages to run the front end/UI of the application.
Public: This folder contains some HTML files for other pages like help and utilities along with the manifest.Json file that specifies how to launch the application.
src: Contains the javascript files that contribute to the front end of the application. index.js is configured to be the root of the application. BrowserRouter then navigates the user to App.js which displays the user with the home page.
package.json: contains all the version of all the dependent packages for the front end.
Server:
config: contains db.js which establishes connection with mongodb and default.json which has the connection string.
node_modules: contains all the dependent packages to run the backend server of the application.
calendarModal.js: Defines the schema for the collection which is used to visually display the added event on the calendar below the Add event button.
timesheetModal.js: Defines the schema for the collection which is in the format that will be sent to the desired calendar (outlook,google etc).
index.js: Responsible for the application server's startup, routing, and other functions.
package.json: contains all the version of all the dependent packages for the back end.
2. SOFTWARE AND PACKAGE VERSIONS:
The application is built using the following technologies:

Node.js: A server-side JavaScript runtime. Version: 18.15.0
React: An open source front end library. Version: 18.2.0
MongoDB: A NoSQL database used for storing user data and timesheets. Version: 6.0
Add2Calendar button: A standalone github component that lets us add buttons to our application which can be used to link to calendars. Version: 2.2.5
3. HOW TO RUN THE CODE:
To get started with the application, follow these steps:

Extract the CodeSubmission zip file (OR) Clone the repository: git clone https://github.com/Deepak-Hariharan/Timesheet-application-for-Employees.git and open it in an IDE of your choice. We used VS code for this project
Enter the following connection string in server\config\default.json : "mongodb+srv://deepakhariharan1999:7PCUpiRxs0LwkAps@cluster0.nx9pp8n.mongodb.net/test"
We will need 2 terminals to run the application. One for the front end and one for the back end.
Go to the client folder in one terminal from the root folder. Use the following command to do so:cd client
Then run the following command to install all the packages that the application depends on: npm i (or) npm install
Run the following command to start the react app:npm run start
Go to the server folder in another terminal from the root folder. Use the following command to do so:cd server
Run the following command to install mongo db: npm install mongodb
Then run the following command to install nodemon: npm install nodemon
Then run the following command to start the node server: nodemon index.js
Once above steps are completed, the application will run on localhost:3000 and open on a new browser window
4. TESTING
This code was tested in the following ways:

Different types of inputs in the form.
Adding to all types of calendars.
Different dates (past and future dates).
Muliple event entries to the database at the same time.
The code worked seamlessly in all the above tests.

5. KNOWN ISSUES
Adding an event doesn't reflect on the visual calendar that is present just below the "Add event" button. The calendar performs a get operation on the database and displays the events. Unable to start the application with the login page as root.

6. SOURCES, REFERENCES, and ATTRIBUTIONS
React big calendar: https://www.npmjs.com/package/react-big-calendar
Connection to mongoDB with Node server: https://www.mongodb.com/blog/post/quick-start-nodejs-mongodb-how-to-get-connected-to-your-database
Add to calendar web component: https://github.com/add2cal/add-to-calendar-button
7. CONTRIBUTING
If you'd like to contribute to the project, please follow these steps:

Fork the repository.
Create a new branch for your changes: git checkout -b my-feature
Make your changes and commit them: git commit -am 'Add new feature'
Push your changes to the branch: git push origin my-feature
Create a pull request and describe your changes.
8. Get Help
If you have any issues or questions, please contact us.
Deepak: deepakhariharan1999@gmail.com
Yutong: yutongy998@gmail.com
