# CSCA5622 Supervised Machine Learning Final Project
In our globalized world, new genres are constantly forming and merging, and song placement into one or more of these categories is increasingly debatable. 

But that doesn't stop us from trying. After all, there is high demand and incentive to categorize music to best cater to millions of music streaming service subscribers.

Humans can easily identify song genres within seconds of hearing a new piece of music. This categorization allows us to group songs by genre and create organized music playlists and libraries. _How well can supervised machine learning classification automate this?_
<hr>

In Part 1, this project uses the __Spotipy API__ to retrieve the songs and their metadata, which includes both __acoustic features__ (like loudness, tempo, key) and what Spotify calls __"psychoacoustic" features__ (like Danceability, Energy, Instrumentalness, Liveness, Valence). All of these metrics are on a 0-1 scale, and we will test __10 genre__ categories containing __100 songs__ each.

The ten genres in the Spotify part of the project are:
1. rap/hip-hop
2. blues
3. classical
4. country
5. electronic dance music (EDM)
6. metal
7. pop
8. reggaeton
9. qawwali
10. rock

In Part 2, we explores another source of song data:  __mel spectrograms__. These are images generated from the transformed and scaled waveform of a song, and may contain a more complete outlook of the song's compositon beyond the summarizing metrics,  thus improving model accuracy. 

More specifically, mel-spectrograms are a visualization of the soundwave amplitudes of a song, after applying a fast Fourier transform to change the scale from time to frequency, and scaling the upper and lower frequencies to better match the perception of the human ear (mel scale).

Unfortunately, 3 of the Spotify categories lack good GTZAN counterparts (genres 5,8, and 9). This means we will test  __7 genre__ categories containing __100 songs__ each here.

Mel spectrograms are sourced from the GTZAN dataset on Kaggle:

Olteanu, Andrada. “GTZAN Dataset - Music Genre Classification.” Www.kaggle.com, 2019, www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification.

In both parts, the training and test data will be determined with an 80:20 split, and then 4 machine learning models will be tested: __logistic regression (LR)__, __random forest (RF)__, __k-nearest neighbors (KNN)__, and a __decision tree (DT)__. 

Let's get started!
<hr>
