# 21_days_Saikrishna-Karra
Beginner. Have an idea about python.

Saikrishna Karra KJSCE SY COMPS.Excited to learn Datascience and embark on this journey.
Day 1: Created a GIT HUB account and a repository.
Day 2:Revised the basics of Python.
Day 3:Revised loops,Regex and functions of Python.
Day 4:Revised Inheritance and Classes in Python.
Day 5:Revised File Handling and Exception Handling in Python.
Day 6:Finished Python revision completely.
Day 7:Understood roughly Numpy Arrays and Vectors.
Day 8:Gained a lot more clarity on Numpy.
Day 9:Watched vids on Pandas.
Day 10:Understood Pandas better.
Day 11:Did study more on Pandas.
Day 12:Watched videos on Matplotlib
Day 13:Revised Numpy.
Day 14:Revised Pandas.
Day 15:Revised Mathplotlib
Day 16:Revising stuff and going through vids of the same.
Day 17:Watched videos on seaborn
Day 18:Revised seaborn.
Day 19:Revising stuff.
Day 20:Revising seaborn again.
Day 21:Ready for doing a project.Have completed the revision.

 Project:
 import matplotlib.pyplot as plt
import pandas as pd
import numpy as np
##Pandas
netflix=pd.read_csv('netflix_titles.csv')
print(netflix)
print(netflix.columns)
print(netflix[['type']])
print(netflix.iloc[0:4])
##for index, row in netflix.iterrows():
    ##print(index, row['title'])
print(netflix.loc[netflix['rating'] == "R"])
print(netflix.iloc[2,1])
print(netflix.sort_values(['type'],ascending=True))
new_netflix = netflix.loc[(netflix['type'] == 'TV Show') & (netflix['country'] == 'United States') & (netflix['rating'] =='R')]

new_netflix.reset_index(drop=True)

print(new_netflix)
new_netflix.to_csv('net.csv')
## Matplotlib
Ng = pd.read_csv('netflix_titles.csv')
Ng = pd.read_csv('netflix_titles.csv')
plt.hist(Ng.release_year)
plt.show()

OUTPUT:
    show_id     type                                    title           director  ... rating   duration                                          listed_in                                        description
0         s1  TV Show                                       3%                NaN  ...  TV-MA  4 Seasons  International TV Shows, TV Dramas, TV Sci-Fi &...  In a future where the elite inhabit an island ...
1         s2    Movie                                    07:19  Jorge Michel Grau  ...  TV-MA     93 min                       Dramas, International Movies  After a devastating earthquake hits Mexico Cit...
2         s3    Movie                                    23:59       Gilbert Chan  ...      R     78 min                Horror Movies, International Movies  When an army recruit is found dead, his fellow...
3         s4    Movie                                        9        Shane Acker  ...  PG-13     80 min  Action & Adventure, Independent Movies, Sci-Fi...  In a postapocalyptic world, rag-doll robots hi...
4         s5    Movie                                       21     Robert Luketic  ...  PG-13    123 min                                             Dramas  A brilliant group of students become card-coun...
...      ...      ...                                      ...                ...  ...    ...        ...                                                ...                                                ...
7782   s7783    Movie                                     Zozo        Josef Fares  ...  TV-MA     99 min                       Dramas, International Movies  When Lebanon's Civil War deprives Zozo of his ...
7783   s7784    Movie                                   Zubaan        Mozez Singh  ...  TV-14    111 min     Dramas, International Movies, Music & Musicals  A scrappy but poor boy worms his way into a ty...
7784   s7785    Movie                        Zulu Man in Japan                NaN  ...  TV-MA     44 min  Documentaries, International Movies, Music & M...  In this documentary, South African rapper Nast...
7785   s7786  TV Show                    Zumbo's Just Desserts                NaN  ...  TV-PG   1 Season                 International TV Shows, Reality TV  Dessert wizard Adriano Zumbo looks for the nex...
7786   s7787    Movie  ZZ TOP: THAT LITTLE OL' BAND FROM TEXAS           Sam Dunn  ...  TV-MA     90 min                    Documentaries, Music & Musicals  This documentary delves into the mystique behi...

[7787 rows x 12 columns]
Index(['show_id', 'type', 'title', 'director', 'cast', 'country', 'date_added',
       'release_year', 'rating', 'duration', 'listed_in', 'description'],      
      dtype='object')
         type
0     TV Show
1       Movie
2       Movie
3       Movie
4       Movie
...       ...
7782    Movie
7783    Movie
7784    Movie
7785  TV Show
7786    Movie

[7787 rows x 1 columns]
  show_id     type  title           director  ... rating   duration                                          listed_in                                        description
0      s1  TV Show     3%                NaN  ...  TV-MA  4 Seasons  International TV Shows, TV Dramas, TV Sci-Fi &...  In a future where the elite inhabit an island ...
1      s2    Movie  07:19  Jorge Michel Grau  ...  TV-MA     93 min                       Dramas, International Movies  After a devastating earthquake hits Mexico Cit...
2      s3    Movie  23:59       Gilbert Chan  ...      R     78 min                Horror Movies, International Movies  When an army recruit is found dead, his fellow...
3      s4    Movie      9        Shane Acker  ...  PG-13     80 min  Action & Adventure, Independent Movies, Sci-Fi...  In a postapocalyptic world, rag-doll robots hi...

[4 rows x 12 columns]
     show_id   type                       title         director  ... rating duration                                        listed_in                                        description
2         s3  Movie                       23:59     Gilbert Chan  ...      R   78 min              Horror Movies, International Movies  When an army recruit is found dead, his fellow...
7         s8  Movie                         187   Kevin Reynolds  ...      R  119 min                                           Dramas  After one of his high school students attacks ...
14       s15  Movie                        3022       John Suits  ...      R   91 min  Independent Movies, Sci-Fi & Fantasy, Thrillers  Stranded when the Earth is suddenly destroyed ...
17       s18  Movie                      22-Jul  Paul Greengrass  ...      R  144 min                                Dramas, Thrillers  After devastating terror attacks in Norway, a ...
65       s66  Movie                     13 Sins     Daniel Stamm  ...      R   93 min                         Horror Movies, Thrillers  A man agrees to appear on a game show with a $...
...      ...    ...                         ...              ...  ...    ...      ...                                              ...                                                ...
7710   s7711  Movie               Yes, God, Yes      Karen Maine  ...      R   78 min             Comedies, Dramas, Independent Movies  A devoutly religious teen grapples with her ow...
7736   s7737  Movie                 Young Adult    Jason Reitman  ...      R   94 min             Comedies, Dramas, Independent Movies  When a divorced writer gets a letter from an o...
7758   s7759  Movie  Zack and Miri Make a Porno      Kevin Smith  ...      R  101 min    Comedies, Independent Movies, Romantic Movies  Zack and Miri make and star in an adult film t...
7774   s7775  Movie                      Zodiac    David Fincher  ...      R  158 min                   Cult Movies, Dramas, Thrillers  A political cartoonist, a crime reporter and a...
7778   s7779  Movie                  Zombieland  Ruben Fleischer  ...      R   88 min                          Comedies, Horror Movies  Looking to survive in a world taken over by zo...

[665 rows x 12 columns]
Movie
     show_id     type                                          title            director  ... rating   duration                                          listed_in                                        description
7786   s7787    Movie        ZZ TOP: THAT LITTLE OL' BAND FROM TEXAS            Sam Dunn  ...  TV-MA     90 min                    Documentaries, Music & Musicals  This documentary delves into the mystique behi...
6614   s6615    Movie                                  The Longshots          Fred Durst  ...     PG     95 min                    Comedies, Dramas, Sports Movies  When an 11-year-old girl becomes Pop Warner fo...
3866   s3867    Movie                                       Mahi NRI    Gaurav Bavdankar  ...  TV-14    134 min             Comedies, Dramas, International Movies  A Punjabi man attempts to build a life in Lond...
6615   s6616    Movie                            The Look of Silence  Joshua Oppenheimer  ...  PG-13    103 min                Documentaries, International Movies  In a society terrorized into silence, the brot...
6616   s6617    Movie  The Lord of the Rings: The Return of the King       Peter Jackson  ...  PG-13    201 min               Action & Adventure, Sci-Fi & Fantasy  Aragorn is revealed as the heir to the ancient...
...      ...      ...                                            ...                 ...  ...    ...        ...                                                ...                                                ...
4019   s4020  TV Show                                      Megalobox                 NaN  ...  TV-MA   1 Season               Anime Series, International TV Shows  Created for the 50th anniversary of manga "Ash...
4020   s4021  TV Show                                   MegaTruckers                 NaN  ...  TV-PG   1 Season                                         Reality TV  This reality ride-along offers a glimpse into ...
4024   s4025  TV Show               Melodies of Life - Born This Way                 NaN  ...  TV-14   1 Season  International TV Shows, Romantic TV Shows, TV ...  A celebrated pastry chef and his fellow staff ...
3951   s3952  TV Show                                           Mars       Everardo Gout  ...  TV-PG  2 Seasons         Docuseries, Science & Nature TV, TV Dramas  Fact meets fiction in this docudrama chronicli...
3893   s3894  TV Show                                       Man Down                 NaN  ...  TV-MA  4 Seasons                      British TV Shows, TV Comedies  A childish idiot trapped in an adult's body, s...

[7787 rows x 12 columns]
Empty DataFrame
Columns: [show_id, type, title, director, cast, country, date_added, release_year, rating, duration, listed_in, description]
Index: []

Pic for graph:
![Screenshot (1266)](https://user-images.githubusercontent.com/87016222/128032351-fb1ed597-fd4d-4b1e-9fba-758af005558d.png)
