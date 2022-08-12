# Moosic_co_project
Moosic is a little start up that creates curated playlists done by music experts and specialists in old and new trends. Users can subscribe to their website and listen to these playlists through their preferred Music App (be it Spotify, Apple Music, Youtube Music…). They love the fact that their playlists have a personal touch, and that each playlist encapsulates a certain “mood” or “style”.  But business is scaling up fast and the music experts are slow in creating new playlists. They have hired you with a clear mission: use Data Science to add a degree of automatisation to the creation of playlists.

They want you to use a dataset that has been collected from the Spotify API and contains the audio features (tempo, energy, danceability…) for a few thousand songs, and use a basic clustering algorithm such as K-Means to divide the dataset into a few clusters (which will become playlists).

Some of the members of the team are skeptical about these audio features being able to capture the actual “mood” of a song: they feel this is something very subjective that only a human can judge. Others are hopeful that a solution that incorporates Data Science can be even better and create connections between songs that might feel unexpected at first glance, but that ultimately make sense.

Either way, on this first week they expect you to have an initial prototype. No pressure: the playlists don’t have to be perfect, and the company understands that they are at the beginning of a lengthy process. They just have to exist and be presented in front of the experts. Between you and them, a couple of assessments will have to be made:

* Are Spotify’s audio features able to identify “similar songs”, as defined by humanly detectable criteria? When you listen to two rock ballads, two operas or two drum & bass songs, you identify them as similar songs. Are these similarities detectable using the audio features from Spotify?
* Is K-Means a good method to create playlists? Would you stick with this algorithm moving forward, or explore other methods to create playlists?
You are expected to present your clusters to the team and discuss these questions with them by next Friday!

## Finding similar songs the human way
The data that you will use in order to group songs are Spotify’s audio features. Obviously, then, the playlists that will emerge from the clustering algorithm that you will apply are going to be completely determined by whatever information these audio features capture from a song.

A human might find a stark difference between two songs because one has lyrics in English and the other in Portuguese, but as long as you do not capture this information (lyrics’ language) and feed it to the clustering algorithm, these two songs will not be distinguished by that. Inversely, if we were to measure something absurd like the length of the song’s name and include it into the algorithm, it would group songs with short names together, and it is highly likely this similarity would make no sense to a human listening to those short-named songs.

In conclusion, it is important to understand what data is available to you, get a feeling for what it is measuring and try to relate these measures to your own human perceptions.

You can start by reading the descriptions that Spotify provides about their audio features. You will see how some of these measures are well established musical properties (key, mode, tempo…) while others have been created by Spotify’s team of Data Science and Sound Engineering (danceability, energy, valence…).

