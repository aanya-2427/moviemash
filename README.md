# moviemash - Movie Recommending Web App
## Submission for Microsoft Engage 2022 🌟
    
<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#salient-features">Salient Features</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#agile-methodology">Agile Methodology</a>
      <ul>
        <li><a href="#what-is-agile">What is Agile</a></li>
        <li><a href="#how-i-incorporated-agile-methodology-during-the-development-cycle">How I Incorporated Agile Methodology During The Development Cycle</a></li>
      </ul>
    </li>
       <li>
      <a href="#Behind-the-recommendation-engine">Behind the Recommendation Engine</a>
      <ul>
        <li><a href="#content-based-filtering">Content Based Filtering</a></li>
        <li><a href="#similarity-score">Similarity Score</a></li>
        <li><a href="#cosine-similarity">Cosine Similarity</a></li></ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#navigating-through-the-app">Navigating through the App</a></li>
      <ul>
        <li>
            <a href="#sign-up">Sign-Up</a>
          </li>
        <li>
            <a href="#sign-in">Sign-In</a>
          </li>
        <li>
            <a href="#search">Search</a>
          </li>
      <li>
          <a href="#movie-info">Movie-info</a>
          </li>
        <li>
            <a href="#cast-info">Cast-info</a>
          </li>
        <li>
            <a href="#recommendation">Recommendation</a>
          </li>
           <li>
               <a href="#sentiment-analysis">Sentiment Analysis</a>
          </li>
        <li>
            <a href="#movies-by-genre">Movies by Genre</a>
          </li>
        <li>
            <a href="#logout">LogOut</a>
          </li></ul>
          <li><a href="#resources-used">Resources Used</a></li>
          <li><a href="#useful-links">Useful Links</a></li>
          <li><a href="#support-and-contact">Support and Contact</a></li>



     
 
  </ol>
</details>




### About The Project

moviemash is a web application developed for Microsoft Engage 2022. As a part of the program, the mentees were assigned the task to choose a track from the three given tracks. moviemash comes under the third track, Algorithms.In this track we were asked to implement a recommendation engine in the app based on any algorithm of our choice.The main aim of the project is to develop a web application which recommends movies to user based on the movie he  searched at that time with ease of use and simplicity. 

### Salient Features
* User authentication using Firebase 
* Search a movie and get its details like title,genre,runtime,rating,poster
* Recommending movies based on the searched movie at that time


### Built With

![Python](https://img.shields.io/badge/Python-3.8-blueviolet)
It is used for building the recommendation engine and <br>
![Framework](https://img.shields.io/badge/Framework-Flask-red)
It is used in integrating the python code with frontend part.<br>
![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)
 It<br>
![API](https://img.shields.io/badge/Backend-Firebase-pink)
 It<br>
![API](https://img.shields.io/badge/API-TMDB-fcba03)<hr>



<!-- AGILE METHODOLOGY -->
### Agile Methodology

### What is Agile

Agile is a development methodology adopted today in the software industry. Agile promotes teamwork, flexible procedures, and sle-organizing teams.

### How I Incorporated Agile Methodology During The Development Cycle

SCRUM is a subset of Agile, a framework for developing software. SCRUM takes advantage of different techniques to achieve goals in Agile. SCRUM promotes an iterative model where the planning is performed on a very short term. The basic time working unit is the sprint. SCRUM teams always reason in sprints and their planning is limited to sprints.


* Sprint 1 (May 4-May 8): Sprint Planning, Research and Design - Researching about what is recommendation engine, whar its types, how it works, what are the agorithms that streaming platfroms like Netflix,Spotify use for their recommendation engine.

* Sprint 2( May 8- May 12):Searched about various libraries (if needed) for implementing recommendation agorithm.  After finalizing the algorithm to be used for recommendation ,I searched for tutorials, designed a wireframe including the functionalities I want and designed the UI.Build a basic prototype of the web application.

* Sprint 3 (May 12- May 24): Software development and debugging - Started the development process by taking help from medium blogs, Youtube tutorials. Built a web application after the initial prototype using Python, Flask and HTML,CSS and JS for frontend, Firebase for storage of data. Encountered occasional bugs which I debugged timely. Made required changes in the UI and color scheme to make it more eye pleasing.

* Sprint 4 (May 24-May 27): Debugging and adding additional features. Decided to build the recommendation engine using content-based filtering by using similarity score and cosine similairty which recommends movie based on the movie that user searched at that time.Made required changes to integrate the frontend part. Added sign in authentication using Firebase. Also added sentiment analysis of the user reviews by scrapping them from IMDB site.<hr>


### Behind the Recommendation Engine
How does the recommendation system behind the application works? What algorithms it uses for the recommendation part.

 
### Content Based Filtering


### Salient Features
* User authentication using Firebase 
* Search a movie and get its details like title,genre,runtime,rating,poster
* Recommending movies based on the searched movie at that time


### Built With

![Python](https://img.shields.io/badge/Python-3.8-blueviolet)
It is used for building the recommendation engine and <br>
![Framework](https://img.shields.io/badge/Framework-Flask-red)
It is used in integrating the python code with frontend part.<br>
![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)
 It<br>
![API](https://img.shields.io/badge/Backend-Firebase-pink)
 It<br>
![API](https://img.shields.io/badge/API-TMDB-fcba03)<hr>


<!-- INSTALLATIONS -->

## Getting Started
To install and run the project on your local system, following are the requirements:
### Prerequisites
Get your `API` key for further steps. Do so by following the steps mentioned below.

1.Create an account in https://www.themoviedb.org/.
2.Click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. 
3.If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your `API` sidebar once your request is approved.

Install python in your system , if not installed already by selecting according to your system from https://www.python.org/downloads/ site.

## Installation
To use this project, follow the steps below:
1. Clone this repository.
Initialise git on your terminal.

```bash
git init
git clone https://github.com/Aanya74282/moviemash-Engage2022.git
```



2. Install all the libraries mentioned in the [requirements.txt](//////////////) file with the command `pip install -r requirements.txt`
3. Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)
3. Replace YOUR_API_KEY in **both** the places (line no. 15 and 29) of `static/recommend.js` file and hit save.
4. Open your terminal/command prompt from your project directory and run the file `main.py` by executing the command `python main.py`.
5. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
6. Yayy! Your site is deployed now.
    
    <hr>


## Navigating Through The App
### Sign-Up

Sign-Up feature to the web application by providing credentials (name, email and password).

<img src="Images/Login-Screen.png" alt="login screen" width="700"/>

### Sign-In

Sign-In using your email and password registered to the web application  which are saved in firebase.

<img src="Images/Login-Screen.png" alt="login screen" width="700"/>

### Search 

  After logging in, a search input appers where one can search the desired movie from the auto-generated list of movies according to the typed letters.

<img src="Images/Blank-Chat-Window.png" alt="blank chat window" width="700"/>


### Movie-info

Get the details of the searched movie like title, genre, runtime,rating,poster,etc which are fetched using an API by TMDB.

<img src="Images/Video-Call-Welcome-Screen.png" alt="video call welcome screen" width="700"/>

### Cast-info

Get the details of the top castof the searched movie and on clicking the know more button which appears on hovering over them , get infromation about them. 

<img src="Images/Video-Call-Welcome-Screen.png" alt="video call welcome screen" width="700"/>


### Recommendation

Get a list of 10  recommended movies based on the movies searched at that time.Thsi recommendation is done by using the content based filtering on the movies data. Click on those movies to search about them and get their details

<img src="Images/Video-Call-Welcome-Screen.png" alt="video call welcome screen" width="700"/>

### Sentiment Analysis

Get the sentiment analysis of the user reviews which are scraped from IMDB site.

<img src="Images/Video-Call-Welcome-Screen.png" alt="video call welcome screen" width="700"/>

### Movies by Genre

Get a list of movies which are displayed by calling API and display them in decraesing order of popularity.

<img src="Images/Video-Call-Welcome-Screen.png" alt="video call welcome screen" width="700"/>

### LogOut

Click on LOGOUT in navigation bar to log out and it will redirect to the sign-in, sign-up page.

<img src="Images/Video-Call-Welcome-Screen.png" alt="video call welcome screen" width="700"/><hr>

    
    
    
    
## Resources Used

* [Recommendation system medium blog](https://medium.com/fnplus/everything-you-need-to-know-about-recommendation-systems-348cdfccbaf0)
* [How to build a recommendation engine in python? medium blog](https://medium.com/swlh/beginners-guide-to-build-recommendation-system-2bd4a96aa3e)
* [How to use flask to render HTML templates medium blog.](https://medium.com/codex/how-to-serve-html-pages-using-flask-and-jinja-597f0157c298)
 * [How to use firebase for user authentication youtube tutorial](https://www.youtube.com/watch?v=qYER6hAgJik)
 * [How to use extract data from API youtube tutorial](https://medium.com/nerd-for-tech/extracting-data-from-an-api-using-python-38e9fbd2525c)
    <hr>
    

## Useful Links

- [Demo Video](////////////////////////////////////////)
- [Sprint Document](///////////////////////////////////)
- [Design Document](/////////////////////////////////)
    
    <hr>
    
## Support and Contact
Email To: aanya44556@gmail.com
<br/>


    
    














