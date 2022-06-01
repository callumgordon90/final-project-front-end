#  FINAL PROJECT: SOCIAL NETWORK FULL STACK MERN PROJECT. 'THE JOKE VAULT' (Part 2: Front end)

<div align="center">
    <a href>
    </a>
    <img alt="Javascript Version" src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E">
    <img alt="Node Version" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white">
    <img alt="React Version" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB">
    <img alt="Redux Version" src="https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white">
    <img alt="JWT Version" src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white">
    <img alt="HTML Version" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
    <img alt="CSS Version" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
    <img alt="SASS Version" src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white">
    <img alt="Heroku Version" src="https://img.shields.io/badge/Heroku-430098?style=for-the-badge&logo=heroku&logoColor=white"> 
</div>

------------------------------------------------------
Click [here](https://github.com/callumgordon90/final-project-front-end) to see the repository of the final project

-------------------
<br>

# 'The Joke Vault'. Summary of the final project:

# Project requirements:

The task is to create a social network.

In the final project of Bootcamp Full Stack in the frontend part, the student is expected to
to demonstrate all the knowledge acquired throughout the course. To do this, the student will combine the knowledge acquired in JavaScript (React + Hooks). 

The following is a list of all the functionalities that the user will be able to carry out.

* There will be the following functionalities: 
* The option to register and create an account,
* Log in and log out
* Posting content (or links to funny videos or original jokes)
* Commenting on or reacting to content posted by other users
* See what jokes are trending
* Follow and unfollow other users
* View a list of suggested users to follow
Inspect other people's profiles


---------------------------------------------------



## https://github.com/callumgordon90/Proyecto-Final-Backend-GeeksHubsAcademy

***


![Home page logged in](/projectpics/homelogged.jpg)
^A view of the home page when a user is logged in
***

![Home page no logged in](/projectpics/homenotlogged.jpg)
^A view of the homepage when the user is NOT logged in - (follow suggestions do not appear)
***


![Chat thread](/projectpics/chatthread.jpg)
^An example of a chat thread on the main wall of the Joke Vault
***


![Edit profile](/projectpics/editprofile.jpg)
^The 'edit profile' page
***





The application has the following features:
* Users can log in to the application. They can then use the additional functionality of the website to communicate with each other. 
    * Members of the website:
        * View their profile page which welcomes them to the site and summarises their activity.
        * Post messages on the main forum.
        * Like' comments written by other users, and have the ability to view their profiles and activity on the site.




![Register](/projectpics/register.jpg)
^The register page
***

![Suggestions](/projectpics/suggestions.jpg)

^The suggestions section
***

![Trending](/projectpics/trending.jpg)
^The trending page - displaying the posts with the most likes




-------------------------------------



## Pre-requisites of the project to run on your local computer:

* Install **Nodejs** on your computer - which can be downloaded from the official page:
https://nodejs.org/

* Clonea el proyecto en tu ordenador con git bash:
```
$git clone 'url-from-repository'
```

* Install all dependencies with the following command:
```
npm install
```

* Start the server with the following command:
```
npm start
```
***

## Technologies used in the project:

* **react**: We install react in our project:
```
npm install react
```
* **react-router-dom**: We install react-router-dom in our project, so we can switch views in our application:
```
npm install react-router-dom
```
* **axios**: We install axios in our project, so that we can connect to the backend API:
```
npm install axios
```
* ** **redux**: We install redux in our project, so we can use redux (state centralisation):
```
npm install redux
```
* **react-redux**: Install react-redux in our project (link react and redux):
```
npm install react-redux
```

***


# SUMMARY: STRUCTURE OF WHOLE PROJECT


# Front end:


The **src** directory is where the entire application is stored. In this directory you will find the following:

** ** **index.js**: This is the main file. From here you call **<App/>**, which is where the whole application will run.

**app.js**: In this file the different **Containers** of the application (views) are managed.

***


* **Actions**: En este directorio almacenamos toda la configuración redux de la aplicación.
    * **post.actions.js**: This file contains the general state of the application.
    * **user.actions.js**: This file contains the general state of the application.
    * **users.actions.js**: This file contains the general state of the application.
    

***

* **Components**: En este directorio almacenamos toda la configuración redux de la aplicación.
    * **AppContext.js**: This file contains the general state of the application.
    * **LeftNav.js**: This file contains the general state of the application.
    * **Navbar.js**: This file contains the general state of the application.
    * **Thread.js**: This file contains the general state of the application.
    * **tools.js**: This file contains the general state of the application.
    * **Trends.js**: This file contains the general state of the application.
  
* **Components/Log**
    * **index.js**: This file contains the general state of the application.
    * **Logout.js**: This file contains the general state of the application.
    * **SignInForm.js**: This file contains the general state of the application.
    * **SignUpForm.js**: This file contains the general state of the application.
  
  **Components/Post**
    * **Card.js**: This file contains the general state of the application.
    * **CardComments.js**: This file contains the general state of the application.
    * **DeleteCard.js**: This file contains the general state of the application.
    * **EditDeleteComment.js**: This file contains the general state of the application.
    * **LikeButton.js**: This file contains the general state of the application.
    * **NewPostForm.js**: This file contains the general state of the application.


  **Components/Profile**
    * **FollowHandler.js**: This file contains the general state of the application.
    * **FriendsHint.js**: This file contains the general state of the application.
    * **UpdateProfile.js**: This file contains the general state of the application.
    * **UpdateImg.js**: This file contains the general state of the application.


  **Components/Routes**
    * **index.js**: This file contains the general state of the application.
    
***



* **Pages**: This directory is where the different views will be stored:
    * **Home.js**: In this view the user can edit their profile.
    * **Profile.js**: In this view the user can edit their profile.
    * **Trending.js**: In this view the user can edit their profile.

***

* **Reducers**: This directory stores all components that will be used in all views:

    * **allPost.reducer.js**: A border that appears at the top at all times.
    * **error.reducer.js**: A section on the side that presents the different links to various pages.
    * **index.js**: A section on the side that presents the different links to various pages.
    * **post.reducer.js**: A section on the side that presents the different links to various pages.
    * **trending.reducer.js**: A section on the side that presents the different links to various pages.
    * **user.reducer.js**: A section on the side that presents the different links to various pages.
    * **users.reducer.js**: A section on the side that presents the different links to various pages.
   

-----------------------------------

by Callum **Gordon**
