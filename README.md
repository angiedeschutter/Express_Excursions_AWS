# Project Express-Excursion
Express Excusrions is a website that allows users to post about a travel destination so other can view when searching for their next adventure.  

## Descripton
The user can select the destination tab and look view other users' post that is sorted by continent.  When the destination is selcted a descritption, location, date visited, author, and picture are shown on that destiantion's page.  The destination can be edited or deleted on the same page.  On the destinations page, a user could add a new destination to the site by clicking 'add destination'.  The user will be redirected to a form page where all availble data is filled out and is posted according to the continent selected.

# Getiing Started

### Dependedncies
    Front-End:
        -react
        -bootstrap
        -sequelize
        -react datepicker

    Back-end:
        -cors
        -dotenv
        -express
        -pg
        -sequelize
        -react datepicker

### Installing
    Fork and clone from https://github.com/angiedeschutter/Express_Excursions_AWS.git

### Executing
    Local operation on separate servers:
        Front end:
            -cd front-end 
            -npm i
            -set up env file
            -npm start

        Back end:
            -cd back-end
            -npm i
            -set up env file
            -nodemon 

        Run from build file on back-end:
            -cd back-end
            -npm i
            -NODE_ENV=production PORT=8000 node index.js

## Contributors
    This was started as a group project for the Milestone 2 project for the UNLV Software Development Bootcamp group #3.


## API (http://localhost:5000/)
    | Method | Path                                 | Purpose                                   |
    | ------ | ------------------------------------ | ----------------------------------------- |
    | GET    | /                                    | Home page                                 |
    | GET    | /destinations                        | Find all destinations                     |
    | GET    | /destinations/:name                  | Find one destination place                |
    | POST   | /destinations                        | Create new destination                    |
    | PUT    | /destinations/:name                  | Update a  destination                     |
    | DELETE | /destinations/:name                  | Delete a  destination                     |
    | GET    | /continents/:continent_name          | Find all destinations for that continent  |
 

## API (http://localhost:3000/)
    | Path                | Component            | Purpose                                             |
    | ------------------- | ---------------------| --------------------------------------------------- |
    | /                   | 'Home.js'            | Home page                                           |
    | /continents         | 'Contients.js'       | Make a list of contients                            |
    | /about              | 'About.js'           | About page                                          |
    | /continents/:name   | 'Destinations.js'    | Create a list of destinations filtered by continent |
    | /destinations/:name | 'Destination.js'     | Details for a specific destination                  | 
    | /newdestination     | 'NewDestination.js'  | Creates a new destination form                      |
    | /edit/:name         | 'Edit.js'            | Edits a new destination form                        |
 
## Change log