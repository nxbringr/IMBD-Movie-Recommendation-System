# IMBD-Movie-Recommendation-System

# What are recommendation systems/engines?
It is a type of information filtering systems that filters the data using different algorithms to improve the quality of search results (recommendations) by providing items that are most relevant items to users based on the item serached or are related to the search history of the user.
The following are the types of recommendation system uses:-
### 1. Demographic Filtering
They offer generalized recommendations to every user, based on item's popularity and/or genre. The System recommends the same items to users with similar demographic features. Since each user is different , this approach is considered to be too simple. The basic idea behind this system is that items that are more popular and critically acclaimed will have a higher probability of being liked by the average audience.

### 2. Content Based Filtering

It recommends the user items that the user himself has previously liked. Eg, someone likes "Person Of Interest" series then the user will be recommended series from alike genre/plot. 

Two types of vectors are maintained by the recommendation system:
* Profile Vector - A vector containing the past behavior of the user,  i.e. the movies liked/disliked by the user and the ratings given by them. 
* Item Vector - Item vector contains the details of each item, say for movie it will store genre, cast, director, etc.

It then finds the Cosing Similarity, i.e., the cosine of the angle between the profile vector and the item vector.

This value ranges between -1 to 1.  Based on cosine distance items are arranges in descening order.


###  3. Collaborative Filtering
This system matches persons with similar interests and provides recommendations based on this matching. Collaborative filters do not require item metadata like its content-based counterparts. 

##### Example - 
If person A likes 3 movies, say Interstellar, Inception and Predestination, and person B likes Inception, Predestination and The Prestige, then they have almost similar interests. We can say with some certainty that A should like The Prestige and B should like Interstellar. 

The collaborative filtering algorithm uses “User Behavior” for recommending items. This is one of the most commonly used algorithms in the industry as it is not dependent on any additional information. 

