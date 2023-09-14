## Collaborative Filtering and Deep Learning-Based Recommender System
## Purpose
This is an initial project of music recommend system, which includes normal and weighted distances algorithms to generate recommendations.

## Data resource
The dataset is from Kaggle, you may access download the dataset from this site: 

https://www.kaggle.com/datasets/vatsalmavani/spotify-dataset

## Spotify credential
You must create an account on Spotify for Developer by this site: https://developer.spotify.com/

You must get your own client id and client secret and replace `clientId` and `clientSecret` on cell 8.

## Implementation
The main function is 

`recommend_songs(song_list, spotify_data, dist_algo=None, super_like=None, n_songs=10)`
1. `song_list`: a song that you want to get recommendation.
2. `spotify_data`: whole dataset from Spotify, generating recommendations from this reference
3. `dist_algo`: default is None, but you must choose a distance algorithm, includes cosine, euclidean, manhattan, braycurtis, and canberra.
4. `super_like`: optional, default is None. The acceptable type is list of integer(s), and it will raise error if the input is not a list.
5. `n_songs`: default is 10. The number of recommended songs.

Documentation of distance algorithms: https://docs.scipy.org/doc/scipy/reference/spatial.distance.html
