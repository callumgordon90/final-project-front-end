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


* **Actions**: In this directory we keep all of the configuration of the application.
    * **post.actions.js**: All of the post actions are contained here
    * **user.actions.js**: All of the single user actions are contained here
    * **users.actions.js**: All of the multiple user actions are contained here
    

***

* **Components**: In this directory we see all of the components that we use in all of the views:
    * **AppContext.js**: The 'create context' function
    * **LeftNav.js**: The navigator bar on the left hand side. Connects the home, trending and profile pages
    * **Navbar.js**: The navbar at the top. Contains logo and logout function
    * **Thread.js**: The wall of posts
    * **tools.js**: Contains the date function
    * **Trends.js**: The most trending posts rated in order of number of likes
  
* **Components/Log**
    * **index.js**: Routes to the sign up and sign in features
    * **Logout.js**: The logout component
    * **SignInForm.js**: For a user to log in to an account
    * **SignUpForm.js**: For a user to sign up and create an account
  
  **Components/Post**
    * **Card.js**: Card containing the various post features
    * **CardComments.js**: Comments on a card
    * **DeleteCard.js**: The component to delete a card (a post on the wall)
    * **EditDeleteComment.js**: The ability to edit a comment
    * **LikeButton.js**: The ability to like the posts of other users
    * **NewPostForm.js**: The template in which a post is made


  **Components/Profile**
    * **FollowHandler.js**: The component to follow and unfollow other users
    * **FriendsHint.js**: The component for other user suggestions
    * **UpdateProfile.js**: The ability to edit and alter your bio or photo
    * **UpdateImg.js**: The component to upload a profile picture


  **Components/Routes**
    * **index.js**: Routes all components
    
***



* **Pages**: This directory is where the different views  of a page will be stored:
    * **Home.js**: This is the home page of the website
    * **Profile.js**: This is the profile page of the website
    * **Trending.js**: This is the trending page of the website

***

* **Reducers**: Reducers modify the state 
  
    * **allPost.reducer.js**: Reducer for all of the posts on the wall
    * **error.reducer.js**: The reducer for errors 
    * **index.js**: Routes all of the other reducers
    * **post.reducer.js**: Changes the state of posts
    * **trending.reducer.js**: Alters the state of trending posts based on likes
    * **user.reducer.js**: The reducer for a single user
    * **users.reducer.js**: The reducer for all users
   

-----------------------------------

**by Callum Gordon**
