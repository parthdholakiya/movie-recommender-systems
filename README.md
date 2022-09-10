# movie-recommender-systems
Recommender System is a system that seeks to predict or filter preferences according to the user’s choices. Recommender systems are utilized in a variety of areas including movies, music, news, books, research articles, search queries, social tags, and products in general. 

![image](https://user-images.githubusercontent.com/94167271/189485447-be5fdeda-2ecb-47dd-909a-0340d7a67a9c.png)


### Recommender systems produce a list of recommendations in any of the two ways – 
 

### Collaborative filtering:

The Collaborative filtering method for recommender systems is a method that is solely based on the past interactions that have been recorded between users and items, in order to produce new recommendations. Collaborative Filtering tends to find what similar users would like and the recommendations to be provided and in order to classify the users into clusters of similar types and recommend each user according to the preference of its cluster. The main idea that governs the collaborative methods is that through past user-item interactions when processed through the system, it becomes sufficient to detect similar users or similar items to make predictions based on these estimated facts and insights. 

Such memory-based approaches directly work with the values of recorded interactions or data and are essentially core based on nearest neighbours search, i.e finding the closest users from a user of interest and suggest the most popular items among these neighbours. The created model approaches assuming there is an underlying “generative” insight that explains the user-item interactions and tries to discover it in order to make new predictions. It recommends an item to user A based on the interests of a similar user B. Furthermore, the embeddings can be learned automatically, without relying on hand-engineering of features. The collaborative filtering method does not need the features of the items to be given. Every user and item is described by a feature vector or embedding. 

The standard method used by Collaborative Filtering is known as the Nearest Neighborhood algorithm. There are several types of filtering such as user-based and Item-based Collaborative Filtering. Considering an example of User-based Collaborative Filtering, If we have an n × m matrix of ratings, with user u, i = 1, …n, and item p, j=1, …m. and we want to predict the rating r if the target user i did not watch/rate an item j. The process is to calculate the similarities between target user i and all other users will be to select the top X similar users and take the weighted average of ratings from these X users with similarities as weights. 

### Challenges with Collaborative Filtering

The only issue with this method is that the prediction of the model for a given user, item pair is the dot product of the corresponding embeddings. So, if an item is not seen during training, the system cannot generally create an embedding for it and hence cannot query the model with this item. This issue is known as the cold-start problem.

### Content-based filtering: 

The content-based approach uses additional information about users and/or items. This filtering method uses item features to recommend other items similar to what the user likes and also based on their previous actions or explicit feedback. If we consider the example for a movies recommender system, the additional information can be, the age, the sex, the job or any other personal information for users as well as the category, the main actors, the duration or other characteristics for the movies i.e the items. 

The main idea of content-based methods is to try to build a model, based on the available “features”, that explain the observed user-item interactions. Still considering users and movies, we can also create the model in such a way that it could provide us with an insight into why so is happening. Such a model helps us in making new predictions for a user pretty easily, with just a look at the profile of this user and based on its information, to determine relevant movies to suggest. 

We can make use of a Utility Matrix for Content-Based Methods. A Utility Matrix can help signify the user’s preference for certain items. With the data gathered from the user, we can find a relation between the items which are liked by the user as well as those which are disliked, for this purpose the utility matrix can be put to best use. We assign a particular value to each user-item pair, this value is known as the degree of preference and a matrix of the user is drawn with the respective items to identify their preference relationship. 

### Challenges faced with Content-based filtering

Content-based methods seem to suffer far less from the cold start problem than collaborative approaches because new users or items can be described by their characteristics i.e the content and so relevant suggestions can be done for these new entities. Only new users or items with previously unseen features will logically suffer from this drawback, but once the system is trained enough, this has little to no chance to happen. Basically, it hypothesizes that if a user was interested in an item in the past, they will once again be interested in the same thing in the future. Similar items are usually grouped based on their features. User profiles are constructed using historical interactions or by explicitly asking users about their interests. There are other systems, not considered purely content-based, which utilize user personal and social data.

![image](https://user-images.githubusercontent.com/94167271/189485536-30c03b39-f100-4271-afa0-c832ab83b571.png)


### Hybrid Recommendation 

A hybrid recommendation system is a special type of recommendation system which can be considered as the combination of the content and collaborative filtering method. Combining collaborative and content-based filtering together may help in overcoming the shortcoming we are facing at using them separately and also can be more effective in some cases. Hybrid recommender system approaches can be implemented in various ways like by using content and collaborative-based methods to generate predictions separately and then combining the prediction or we can just add the capabilities of collaborative-based methods to a content-based approach (and vice versa). 

![image](https://user-images.githubusercontent.com/94167271/189485000-db0d4770-4b4b-4cdb-8627-c2ed1a4d4cb2.png)


There are several studies that compare the performance of the conventional approaches with the hybrid methods and say that by using the hybrid methods we can generate more accurate recommendations.

#### I would like to mention some excellent refereces that I learned from

1, https://analyticsindiamag.com/collaborative-filtering-vs-content-based-filtering-for-recommender-systems/
