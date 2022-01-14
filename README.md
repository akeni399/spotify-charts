# spotify-charts
<b> Introduction: </b>
<br>
I found a <a href="https://www.kaggle.com/bartomiejczyewski/spotify-top-200-weekly-global-20172021">dataset</a> on Kaggle that documented the global top 200 songs from Spotify every week and downloaded the .csv file of the data. I organized the data into separate tables, renaming information, and made it easier for me to understand. 

<img src="https://user-images.githubusercontent.com/96144192/149042027-1aefd390-0643-4956-a4e6-1ff493b10588.png" width="650" height="350"/>


I put information about artists in one table, such as their number of followers, and created the other table based on song details, such as length, minutes streamed, and explicit content.
I created columns in both tables that kept track of the serial number (a.artist_num and (s.track_number) making one of them a primary key, allowing me to create a relationship between both tables. 

<i> Query 1</i>
The query showed that Post Malone had the highest number of occurences in the top 30 of the global charts at 127 occurences. However, as query 2 showed, this wasn't consistent with occurences in the global top 200. Ed Sheeran had the most occurences, with 1320, meaning that while Ed Sheeran ends up in the top 200 fairly often, he doesn't land in the top 10 quite as often as other artists.  

Next, I picked an artist at random, Ariana Grande, and used GROUP BY to find her highest ranking album Sweetener, and the difference between her next highest ranked album, Positions. Sweetener was on the charts 120 times, while Positions was at 86. 

Next, I wanted to see the position an artist ranks on the charts affects the number of followers they had on Spotify, comparing artists' ranks and follower_num. I found that while the trend is fairly consistent with top ranked artists having more follower (eg. Ed Sheeran), there are outliers such as 'Thirty Seconds to Mars' while have a hig follower count despite being lower in the rankings. 

I also wanted to see if explicit content in songs affected their position on the charts, and whether listener displayed an outright preference. In query 6, I used the COUNT function to determine the number of songs that ranked #1 that had explicit content. I found that there was not much of a difference (121 explicit songs and 100 non-explicit songs).
