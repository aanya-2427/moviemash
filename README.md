# moviemash - Movie Recommending Web App
<img src="ReadMe_images/logo3.png" alt="Sign-Up screen" width="700"/>

## Submission for Microsoft Engage 2022 🌟
    
# TABLE OF CONTENTS
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
               <a href="#home">Home</a>
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
          <li><a href="#sources-of-the-datasets">Sources of the Datasets</a></li>
          <li><a href="#useful-links">Useful Links</a></li>
          <li><a href="#support-and-contact">Support and Contact</a></li>



     
 
  </ol>
</details><hr>




### About The Project

moviemash is a web application developed for Microsoft Engage 2022. As a part of the program, the mentees were assigned the task to choose a track from the three given tracks. moviemash comes under the third track, Algorithms.In this track we were asked to implement a recommendation engine in the app based on any algorithm of our choice.The main aim of the project is to develop a web application which recommends movies to user based on the movie he  searched at that time with ease of use and simplicity. 

### Salient Features
* User authentication using Firebase 
* Search a movie and get its details like title,genre,runtime,rating,poster
* Recommending movies based on the searched movie at that time


### Built With

![Python](https://img.shields.io/badge/Python-3.8-blueviolet)
It is used for data processing for the recommendation engine  <br>
![Framework](https://img.shields.io/badge/Framework-Flask-red)
It is used in integrating the python code with frontend part.<br>
![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)
 These are used for styling the website(frontend).<br>
![API](https://img.shields.io/badge/Backend-Firebase-pink)
 It is used for storing the registered user's credentials(email).<hr>[(Back to top)](#table-of-contents)



<!-- AGILE METHODOLOGY -->
### Agile Methodology

### What is Agile

Agile is a development methodology adopted today in the software industry. Agile promotes teamwork, flexible procedures, and sle-organizing teams.

### How I Incorporated Agile Methodology During The Development Cycle

SCRUM is a subset of Agile, a framework for developing software. SCRUM takes advantage of different techniques to achieve goals in Agile. SCRUM promotes an iterative model where the planning is performed on a very short term. The basic time working unit is the sprint. SCRUM teams always reason in sprints and their planning is limited to sprints.


* Sprint 1 (May 4-May 8): <strong>Sprint Planning and Research - </strong> Researching about what is recommendation engine, whar its types, how it works, what are the agorithms that streaming platfroms like Netflix,Spotify use for their recommendation engine.

* Sprint 2( May 8- May 12):<strong>Design phase -</strong> Various libraries(if needed) for implementing recommendation agorithm.  After finalizing the algorithm to be used for recommendation ,I searched for tutorials, designed a wireframe including the functionalities I want and designed the UI.Build a basic prototype of the web application.

* Sprint 3 (May 12- May 24): <strong>Build phase -</strong> Started the development process by taking help from medium blogs, Youtube tutorials. Built a web application after the initial prototype using Python, Flask and HTML,CSS and JS for frontend, Firebase for storage of data. Encountered occasional bugs which I debugged timely. Made required changes in the UI and color scheme to make it more eye pleasing.

* Sprint 4 (May 24-May 27): <strong>Testing Phase -</strong>Debugging and adding additional features. Decided to build the recommendation engine using content-based filtering by using similarity score and cosine similairty which recommends movie based on the movie that user searched at that time.Made required changes to integrate the frontend part. Added sign in authentication using Firebase. Also added sentiment analysis of the user reviews by scrapping them from IMDB site.<hr>[(Back to top)](#table-of-contents)


### Behind the Recommendation Engine
How does the recommendation system behind the application works? What algorithms it uses for the recommendation part.

 
### Content Based Filtering
Content-based Filtering analyses the nature of each item and aims to find the insights of the data to identify the user preferences. Basically content recommenders rely on item features to make recommendations. Examples of this features include User generated tags on movies, Item color, Text description, User review of an item, Genre, Director, Description, Actors of a Movie etc. The general idea behind these recommender systems is that if a person likes a particular item, he or she will also like an item that is similar to it. In other words, these algorithms try to recommend items that are similar to those that a user liked in the past. This can be seen in applications like Netflix, Facebook Watch which recommend the next movie or video based on the Director, Hero etc. In this post I have used Content-based Filtering to find the recommendations of the movies. The recommendation system build with title, cast, director, keywords, genres features in the dataset.

### Similarity Score
How does it decide which item is most similar to the item user likes? Here come the similarity scores.

It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
### Cosine Similarity
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.<hr>[(Back to top)](#table-of-contents)



<!-- INSTALLATIONS -->

## Getting Started
To install and run the project on your local system, following are the requirements:
### Prerequisites
1.Get your `API` key for further steps. Do so by following the steps mentioned below.

Create an account in https://www.themoviedb.org/.<br>
Click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key.<br> 
If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your `API` sidebar once your request is approved.<br>

2.Install python in your system , if not installed already by selecting according to your system from https://www.python.org/downloads/ site.

## Installation
To use this project, follow the steps below:
1. Clone this repository.
Initialise git on your terminal.

```bash
git init
git clone https://github.com/Aanya74282/moviemash-Engage2022.git
```



2. Install all the libraries mentioned in the [requirements.txt]file with the command `pip install -r requirements.txt`
3. Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)
4. Replace YOUR_API_KEY in **both** the places (line no. 15 and 35) of `static/recommend.js` file,in line no.8 of `api.js` and hit save.
5. Open your terminal/command prompt from your project directory and run the file `main.py` by executing the command `python main.py`.
6. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
7. Yayy! Your site is deployed now.
    
    <hr>
[(Back to top)](#table-of-contents)

## Navigating Through The App
### Sign-Up

Sign-Up feature to the web application by providing credentials (name, email and password).

<img src="ReadMe_images/ss2.png" alt="Sign-Up screen" width="700"/>

### Sign-In

Sign-In using your email and password registered to the web application  which are saved in firebase.

<img src="ReadMe_images/ss1.png" alt="Sign-In screen" width="700"/>

### Home
The Home window appears where the users can search for the desired movies, scroll through their favourite movies  sorted according to their genres.

<img src="ReadMe_images/ss10.png" alt="Home screen" width="700"/>


### Search 

 After logging in, a search input appears where one can search the desired movie with the autocomplete feature and get all the information like title,genres,release etc about that movie..

<img src="ReadMe_images/ss3.png" alt="Search Window" width="700"/>


### Movie-info

Get the details of the searched movie like title, genre, runtime,rating,poster,etc which are fetched using an API by TMDB.

<img src="ReadMe_images/ss4.png" alt="Movie details screen " width="700"/>

### Cast-info

After searching the movie,get the details of the top cast of the searched movie and on clicking the know more button which appears on hovering over them , get information about them. 

<img src="ReadMe_images/ss5.png" alt="Cast info screen" width="700"/>


### Recommendation

Get a list of 10  recommended movies based on the movies searched at that time.This recommendation is done by using the content based filtering on the movies data. Click on those movies to search about them and get their details

<img src="ReadMe_images/ss6.png" alt="Recommended movies screen" width="700"/>

### Sentiment Analysis

Get the sentiment analysis of the user reviews who have already wathced the movie which are scraped from IMDB site.

<img src="ReadMe_images/ss7.png" alt="SEntiment analysis for user reviews screen" width="700"/>

### Movies by Genre

Get a list of movies which are displayed by calling API and display them in decraesing order of popularity.

<img src="ReadMe_images/ss8.png" alt="Movies displayed by genre using API screen" width="700"/>

### LogOut

Click on LOGOUT in navigation bar to log out and it will redirect to the sign-in, sign-up page.

<img src="ReadMe_images/ss9.png" alt="Logout alert screen" width="700"/><hr>[(Back to top)](#table-of-contents)

    
    
    
    
## Resources Used

* [Recommendation system medium blog](https://medium.com/fnplus/everything-you-need-to-know-about-recommendation-systems-348cdfccbaf0)
* [How to build a recommendation engine in python? medium blog](https://medium.com/swlh/beginners-guide-to-build-recommendation-system-2bd4a96aa3e)
* [How to use flask to render HTML templates medium blog.](https://medium.com/codex/how-to-serve-html-pages-using-flask-and-jinja-597f0157c298)
 * [How to use firebase for user authentication youtube tutorial](https://www.youtube.com/watch?v=qYER6hAgJik)
 * [How to use extract data from API youtube tutorial](https://medium.com/nerd-for-tech/extracting-data-from-an-api-using-python-38e9fbd2525c)
    <hr>
[(Back to top)](#table-of-contents)

### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)
<hr>

[(Back to top)](#table-of-contents)

    

## Useful Links

- [Demo Video](https://www.canva.com/design/DAFCGYwNtwE/287BLgqHZRq7XHB5eow5gA/watch?utm_content=DAFCGYwNtwE&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)
- [Sprint Document](https://docs.google.com/presentation/d/1ZL2xV9rMHPZQO7wU06dyqFe26BF8vZiAmNdZpumXXU8/edit?usp=sharing)
- [Design Document](https://docs.google.com/document/d/1D6yE0ieLOIxPs4cC8u-yhh3XCi_-mHArPNS_o6m7qFU/edit?usp=sharing)
    
    <hr>
    
[(Back to top)](#table-of-contents)
    
## Support and Contact
Email To: aanya44556@gmail.com
<br/>
[(Back to top)](#table-of-contents)


    
    














