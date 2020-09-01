# Spotify Recommender Engine

This project is based on the [Kaggle dataset](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks) by [Yamaç Eren Ay](https://www.kaggle.com/yamaerenay). In this project, there are a couple of questions -- both from the author and myself. These are as follows:

## 1. Recommend similar songs based on genre/artist.

### Task Details
Given a number of input from the user (representing that user's preference), I expect to be able to recommend similar songs based on that input. Such recommendation can vary from genre-based and artist-based. 

For example, if a user inputs `Metalcore` as their most preferred genre, the engine might recommend songs belonging to `Hardcore Punk` than it is to recommend `Thrash Metal`, despite they three are of the same primary genre which is metal.

Likewise, if a user inputs `In This Moment` as their most preferred band, the engine might recommend songs from `Black Veil Brides` than it is to recommend ones from `Alice in Chains`, because the two former are more gothic than the latter despite those are of the same primary genre, which is also metal.

One big idea is also to introduce a feature where the engine recommends songs from the same popular playlist -- for example, a videogame soundtrack. This is basically saying: "Because you enjoy song A from a videogame called X. You might enjoy song B from the same videogame"

## 2. Recommend modern-sounding sounds based on time-series analysis

### Task Details
We can also try to analyze the music trends based on the year they're released (i.e. what are the characteristics of music from each decade). For example, both Elton John and Britney Spears are very popular amongst all manner of audiences -- despite they thrive in their own golden age. We try to analyze numerically how do Elton's and Britney's music are represented via numbers.

Then, based on a given year as input, we can then recommend the songs most suited to represent that era. For instance, if an input is the year '1985', we'd want the engine to recommend `Motley Crue` than it is to recommend `Justin Bieber`.

## 3. Recommend songs that two users will both enjoy

### Task Details
The third and probably the hardest question to answer (for me, at least) is to recommend songs based on the preference of two users. For this, I would need to connect to the Spotify Developer API. The input is two different user ID, and the output is songs that they both would most likely enjoy based on their listening habits.

For example, user A frequently listens to upbeat and pop music, while user B frequently listens to classic rock ballads. The recommender engine tries to find the meeting point for both users' preferences, and recommends tracks based on that meeting point.

--- 

### License Agreement

This dataset is licensed under Community Data License Agreement – Sharing, Version 1.0. By using this data, I hereby consent to share any changes, modifications, and deployable models based on this data over the course of this project.

The Community Data License Agreement workgroup under The Linux Foundation is the steward of this Agreement. No one other than the Steward has the right to modify or publish new versions of this Agreement.