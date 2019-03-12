# iTrack
This is a simple web application for tracking mobile phones via a various number of android service installed on the devices that runs in the background. Implemented for CSE334 Internet Programming Course.

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
// web app wireframe
// Home (landing page)
// About (about us page)
// App
    if(!session)
        // login
        getUserDataFromDB
        if(user)
            if(passwordMatch)
                logged in
                redirect to app
            else
                // forgot password feature coming later
    else
        regitser
        redirect to login
        

### Register
The Signup/Register form will appear to the user who will have to enter the necessary fields: Name, Password, Email ID, Mobile Phone Number.<br>
The password field will be hashed by the PHP crypto method and then all the fields will be saved in the database as a record for this user.<br>
This will be followed by receiving a mail including the android service.<br>
![sequence-diagram](https://user-images.githubusercontent.com/25902120/54239924-4b3e6e80-4525-11e9-81ac-60039cef796d.jpeg)

### Login
// hash compare

### Database
// service keep sending to db, frontend requests, backend calls the db, db responds, backend responds
![db-schema](https://user-images.githubusercontent.com/25902120/54239922-4b3e6e80-4525-11e9-8865-4d3060da13cb.jpeg)

## Contributors
[**Mohamed El Ghamry**](https://github.com/Ghamry0x1)<br>
[**Youssed Kembal**](https://github.com/Ghamry0x1)<br>
[**Mostafa Hazem**](https://github.com/mostafa172)<br>
[**Mohamed Hussien**](https://github.com/mohamedhussein98)<br>