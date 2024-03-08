# Book Recommender System 
This project is a simple implementation of a book recommender system using Python. It utilizes two different approaches: popularity-based and collaborative filtering. The code and dataset used in this project are available in this Git repository.

## Table of Contents
**Popularity Based Recommender System**
  - Description: This approach recommends books based on their popularity, determined by the number of ratings and the average rating they have received.
  
**Collaborative Filtering Based Recommender System**
  - Description: Collaborative filtering recommends items based on the preferences of other users. It identifies users who have similar preferences and suggests items that those similar users have liked or interacted with.
### Popularity Based Recommender System: In this approach, we recommend books based on their popularity, which is determined by the number of ratings and the average rating they have received.

### Data Preprocessing: 
We read the books, users, and ratings CSV files and perform some initial data cleaning.
### Data Analysis:
We analyze the dataset to get insights, such as the number of unique users, the number of unique books, and the number of unique ratings.
### Popular Books:
We filter the books with a minimum number of ratings (250 in this case) and sort them by their average rating in descending order.
## Collaborative Filtering Based Recommender System
In this approach, we recommend books based on the ratings given by similar users.

## Data Preprocessing: 
We filter users with a minimum number of ratings (200 in this case) and books with a minimum number of ratings (50 in this case).
## User-Book Rating Matrix:
We create a user-book rating matrix pt where each row represents a user, and each column represents a book. The value in each cell is the rating given by the user to the book.
## Cosine Similarity: 
We calculate the cosine similarity between each pair of books to find similar books based on users' ratings.
## Recommendation Function:  
We create a function recommend(book_name) that takes a book name as input and returns a list of similar books based on cosine similarity.
