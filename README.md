# TS-Song-Popularity-Analysis

### Explored dataset from [here](https://www.kaggle.com/datasets/jarredpriester/taylor-swift-spotify-dataset?select=taylor_swift_spotify.csv) on different TS song features (based on Spotify data of month of September)

### See the notebook + results visualized [here](http://htmlpreview.github.io/?https://github.com/kitkatmia/TS-Song-Popularity-Analysis/blob/main/superior_preview.html)

- Unfortunately, github preview of .ipynb extensions is lacking right now (:disappointed_relieved:), so the best viewing alternative was converting the file to an html file and getting a link to that

### Main parts:

- EDA
- Regression (Linear Regression, SVR, Random Forest, Gradient Boosting, Decision Tree)
- Clustering (DBSCAN)
- And many interesing side tangents

### Main Takeaways

| Question                                                              | Answer                                                                                                                                                                                                                                                                                                                                                                            |
| --------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Can song popularity be predicted based on the spotify given features? | <ul><li>To some extent, yes, but not very reliably</li><li>TS's general popularity with the public is more likely a bigger indicator</li><li>Other important factors that weren't considered here but could have a large effect are the mood of the song (ex: sad, happy, angry), over-arching theme (ex: breakup, love), and genre (ex: ultra pop, country-ish, indie)</li></ul> |
| Will future TS songs be, on average, more popular than current ones?  | <ul><li>Trendline says yes</li><li>But it again depends on general popularity of TS more so than the song numerical features</li></ul>                                                                                                                                                                                                                                            |
| Of the features tested, which ones were the most important?           | <ul><li>Loudness, speechiness, and liveness, respectively</li></ul>                                                                                                                                                                                                                                                                                                               |
| What do the songs clustered look like?                                | <ul><li>Long story short: messy</li><li>Again, solely using technical aspects of a song seem to be a poor indicator of important song characteristics that would affect groupings (ex: I Did Something Bad and Tied Together With A Smile are placed in the same cluster despite being clearly different)</li></ul>                                                               |

### Feature Explanation

Just in case the kaggle link gets taken down, the columns in this dataset are:

**name** - the name of the song

**album** - the name of the album

**release_date** - the day month and year the album was released

**track number** - the order the song appears on the album

**id** - the Spotify id for the song

**uri** - the Spotify uri for the song

**acousticness** - A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.

**danceability** - Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.

**energy** - Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.

**instrumentalness** - Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.

**liveness** - Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.

**loudness** - The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typically range between -60 and 0 db.

**speechiness** - detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.

**tempo** - The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.

**valence** - A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).

**popularity**- the popularity of the song from 0 to 100

**duration_ms** - The duration of the track in milliseconds.
