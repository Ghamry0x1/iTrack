# iTrack
This is a simple web application for tracking mobile phones via a various number of android service installed on the devices that runs in the background. Implemented for CSE334 Internet Programming Course.

## Table of Contents
**[Technologies Used](#technologies-used)**<br>
**[Mockups](#mockups)**<br>
**[Scenarios and Use Cases](#scenarios-and-use-cases)**<br>

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

## Mockups
### Home
![home](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)

### About
![about](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)

### Login
![login](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)

### Register
![register](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)

### App
![app](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)


## Scenarios and Use Cases
![use-case-diagram](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)

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
// form, emailing the service, hashing pass
![sequence-diagram](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)

### Login
// hash compare

### Database
// service keep sending to db, frontend requests, backend calls the db, db responds, backend responds
![db-schema](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)
