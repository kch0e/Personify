# Personify

[Spring 2019] Los Altos Hacks IV - Team Submission

## Inspiration
My partners and I are very musically oriented individuals. We understand that an individual's preference in music says a lot about other aspects of their life, such as personality, mood, and more. We decided to use the Spotify API to gather information regarding a song's musical information and convert that into meaningful statistics that could be compared and analyzed.

## What it does
The application calls the Spotify API and collects the user's top 50 most listened to songs. It then compares the weighted average of the key, mode, acousticness, danceability, energy, instrumentalness, liveness, loudness, speechiness, valence, and tempo of the songs. The results can be used to determine current preferences and trends in pop culture as well as how an individual compares to the societal norm. The terms we use are defined below:

key: The estimated overall key of the track

mode: Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived.

acousticness: A confidence measure from 0.0 to 1.0 of whether the track is acoustic.

danceability: How suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity.

energy: A measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity.

instrumentalness: Predicts whether a track contains no vocals. “Ooh” and “aah” sounds are treated as instrumental in this context.

liveness: Detects the presence of an audience in the recording.

loudness: Detects the presence of an audience in the recording.

speechiness: Detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value.

valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).

tempo: The overall estimated tempo of a track in beats per minute (BPM).

## How we built it
The user authenticates our application through Spotify's OAuth System. We call the API first for all the user's playlists and order the user's songs from most frequently to least frequently listened to. Based on this ordering of songs, we find the statistics mentioned above, using a weighted average to ensure the accuracy of the model. We then conduct a similar call for the top 50 songs currently trending in the US, whose statistics change based on time frame. The information is then represented through a radar graph to observe the similarities and differences between the user's characteristics and the characteristics of the top songs in the nation.

PLEASE NOTE THAT A LARGE NUMBER OF API CALLS NEED TO BE PERFORMED BEFORE THE RESULTS ARE OUTPUTTED. PLEASE WAIT FOR THE RESULTS TO LOAD BEFORE RECLICKING THE SUBMIT BUTTON

## Challenges we ran into
As beginners, we had a large amount of difficulty learning how to use the Spotify API, which we had never learned before. Furthermore, the documentation for the Spotify API was written in HTTPS/HTTP format, and we had to convert this to cURL in order to call the API with our backend language, PHP. We also had the issue of biting off more than we could chew, trying to integrate more features into our product than we really had time for. As a result, we ended up with a product that could've been better in multiple aspects.

## Accomplishments that we're proud of
Learning how to use the Spotify API was definitely very challenging. However, in the end, we were still able to make the calls we were supposed to and come up with a viable product.

## What we learned
We learned a lot about applications of backend technology and also significantly enhanced our frontend development skills. We also gained a significant amount of knowledge regarding machine learning, as the statistics we found with our application of the Spotify API required some machine learning and regression knowledge.

## What's next for Personify
We want to take the data acquired from this project and put it to more practical applications. As of right now, Personify offers a comparision between cultural and and individuals' statistics. We plan on integrating this with other types of information technology, such as sentiment analysis on music lyrics, to analyze information that can be directly applied, instead of inferred.

## Authors
Built by Kevin C, Dylan F, Ethan L - official submission can be found [here.](https://devpost.com/software/personify-iz3px2)
