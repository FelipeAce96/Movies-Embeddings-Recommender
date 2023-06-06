# Movies-Embeddings-Recommender 🎥

A movies recommender based in embeddings.
I used a transformer model from hugging face, the instructor large model to obtain the embeddings from each movie.
The embeddings are calculated using the following prompt:

    MOVIE FEATURES
    TITLE: Toy Story
    COLLECTION: Toy Story Collection
    COMPANY NAME: Pixar Animation Studios
    RELEASED: 1995
    OVREVIEW: Led by Woody, Andy's toys live happily in his room until Andy's birthday brings Buzz Lightyear onto the scene. Afraid of losing his place in Andy's heart, Woody plots against Buzz. But when circumstances separate Buzz and Woody from their owner, the duo eventually learns to put aside their differences.
    GENRES:
      Animation
      Comedy
      Family


## Results

I pass throught a PCA model the embeddings to reduce his dimensionality from 768 to 128 and save some memory.
Save the embeddings and use a KNN model to get the movies close to the one choosed to test.

Test Movie: Batman v Superman: Dawn of Justice 
![image](https://github.com/FelipeAce96/Movies-Embeddings-Recommender/assets/53706252/fabe5445-9caf-471f-b934-0f3ed48b164c)

