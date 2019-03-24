# iTrack
This is a simple user-friendly web application for tracking mobile phones via a various number of android service installed on the devices that runs in the background. We have 2 packages; Personal-use package that supports only 1 mobile phone tracking and it's free, Commercial-use package that supports up to 10 mobile phones tracking. Implemented for CSE334 Internet Programming Course.

## Table of Contents
**[Technologies Used](#technologies-used)**<br>
**[Scenarios and Use Cases](#scenarios-and-use-cases)**<br>
**[Contributors](#contributors)**<br>

## Technologies Used
- [**HTML**](https://en.wikipedia.org/wiki/HTML): Hypertext Markup Language is the standard markup language for creating web pages and web applications.
- [**CSS**](https://en.wikipedia.org/wiki/Cascading_Style_Sheets): Cascading Style Sheets is a style sheet language used for describing the presentation of a document written in a markup language like HTML. 
- [**JavaScript**](https://en.wikipedia.org/wiki/JavaScript): The Programming Language for the Web, that can update and change both HTML and CSS, and also can calculate, manipulate and validate data.
- [**JQuery**](https://en.wikipedia.org/wiki/JQuery): A JavaScript library designed to simplify HTML DOM tree traversal and manipulation, as well as event handling, CSS animation, and Ajax. It is free, open-source software using the permissive MIT License.
- [**Ajax**](https://en.wikipedia.org/wiki/Ajax_(programming)): A set of web development techniques using many web technologies on the client side to create asynchronous web applications. With Ajax, web applications can send and retrieve data from a server asynchronously without interfering with the display and behavior of the existing page.
- [**PHP**](https://en.wikipedia.org/wiki/PHP): Hypertext Preprocessor (PHP) is a programming language for writting servers, allows web developers to create dynamic content that interacts with databases.
- [**MySQL**](https://en.wikipedia.org/wiki/MySQL): Open source relational database management system, that is used to store data inside of it.
- [**Google Maps API**](https://developers.google.com/maps/documentation/): Google APIs is a set of application programming interfaces developed by Google which allow communication with Google Services and their integration to other services.
- [**Android Geo Location Service**](http://to.be.deployed): A simple service that runs in the background on the users's android phone, that keeps sending his geo location periodically.

## Scenarios and Use Cases
![use-case-diagram](https://user-images.githubusercontent.com/25902120/54239921-4aa5d800-4525-11e9-934a-d4dfb02f3522.jpeg)

### Routing
The very start page that the user will face when launching the web application is the landing page (index.html).
There will be a navigation bar that contains 3 links:
- *Home:* Navigates the user to the home page (index.html). 
- *About*: Navigates the user to the about page (about.html) which contains more info and social links of the developing team. 
- *App*: Navigates the user to login/registration page(s). If the user logins' successfully, he will be redirected automatically to the App page (app.html). If not; the login and registartion scenarios proceed.

If user navigates to any page after login, and go back again to the App; no login will be required because a session for this user will be instantiated.
        
### Register
The Signup/Register form will appear to the user who will have to enter the necessary fields: Name, Password, Email ID, Mobile Phone Number.<br>
The password field will be hashed by the PHP crypto method and then all the fields will be saved in the database as a record for this user.<br>
This will be followed by receiving a mail including the android service.<br>
![sequence-diagram](https://user-images.githubusercontent.com/25902120/54239924-4b3e6e80-4525-11e9-81ac-60039cef796d.jpeg)

### Login
1. The user will enter his username and password and then press Login.
2. The form will be submitted and send to our server.
3. The server will get user using his username from the database.
	- If the user exists, the server will continue with step 4.
	- If user does not exist, an error message will be shown for the user, and he will be promoted to try to enter his credentials again or to register.
4. The server will hash the form password using an irreversible hashing function.
5. The server will compare the hashed user password saved in the database with the hashed form password.
	- If matches, the login will be successful, and the user will have access.
	- If does not matches, then an error message will show up telling the user that the entered password was not correct and to retry.

### Database
// service keep sending to db, frontend requests, backend calls the db, db responds, backend responds
![db-schema](https://user-images.githubusercontent.com/25902120/54239922-4b3e6e80-4525-11e9-8865-4d3060da13cb.jpeg)

## Contributors
[**Mohamed El Ghamry**](https://github.com/Ghamry0x1)<br>
[**Youssed Kembal**](https://github.com/YKembal)<br>
[**Mostafa Hazem**](https://github.com/mostafa172)<br>
[**Mohamed Hussien**](https://github.com/mohamedhussein98)<br>