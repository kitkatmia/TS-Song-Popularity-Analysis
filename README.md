# TS-Song-Popularity-Analysis

### Explored dataset from [here](https://www.kaggle.com/datasets/jarredpriester/taylor-swift-spotify-dataset?select=taylor_swift_spotify.csv) on different TS song features (based on Spotify data)

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
