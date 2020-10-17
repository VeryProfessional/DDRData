# The Mathematical Findings of DDR Difficulty Calculators

**Project Background:** This project aims to create datasets and analysis for the game Dance Dance Revolution to create a greater understanding of the difficulty meter in the game. This requires many factors within the game to be taken into account. These included song information, player records, user information, and ordered data. The results were calculated by eyeballing the graphs and picking ranges which stand out. Interpretations are made over whether or not the correlation equals causation in each dataset. 

Additionally, in this project I would like to compare two methods of interpretation: human insight and computer models (to calculate which features will affect the difficulty of the DDR songs). The results can be used to improve the user engagements of the next generations of DDR and the methodology of comparing game features, which can be applied to other human computer interactions and data science researches. The biggest way this project can be improved is by mathematically solving for the data, which would not only be more accurate, but could also prove if there is causation with the trends. While there is some room for improvement, the original goal has been fulfilled.

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/DDR.jpg) [credit](https://www.researchgate.net/figure/Screen-shot-and-description-of-DDR_fig2_220473903)

**Dance Dance Revolution:** Dance Dance Revolution is a music video game series produced by Konami.  Players stand on a "dance platform" or stage and hit colored arrows laid out in a cross with their feet to musical and visual cues. Players are judged by how well they time their dance to the patterns presented to them. The core gameplay involves the player stomping their feet to correspond with the arrows that appear on screen and the beat. During normal gameplay, arrows scroll upwards from the bottom of the screen and pass over a set of stationary arrows near the top. When the scrolling arrows overlap the stationary ones, the player must step on the corresponding arrows on the dance platform, and the player is given a judgement for their accuracy of every streaked notes (From highest to lowest: Marvelous,Perfect, Great, Good, Almost, Miss)

 Freeze Arrows, introduced in MAX, are long green arrows that must be held down until they completely travel through the Step Zone. Each of these arrows awards an "O.K.!" if successfully pressed or an "N.G." when the arrow is released too quickly. An "N.G." decreases the life bar and, starting with X, also breaks any existing combo. X also introduced Shock Arrows, walls of arrows with lightning effects which must be avoided, awarding an "O.K.!" if successfully avoided or an "N.G." if any of the dancer's panels are stepped on. An "N.G." for shock arrows has the same consequences found with freeze arrows, but hitting a shock arrow additionally hides future steps for a short period of time.
 
Successfully hitting the arrows in time with the music fills the "Dance Gauge", or life bar, while failure to do so drains it. If the Dance Gauge is fully exhausted during gameplay, the player will fail the song, and the game will be over. Otherwise, the player is taken to the Results Screen, which rates the player's performance with a letter grade and a numerical score, among other statistics. 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/gameplay.png)


**Process:** The process took a total of eight weeks or sixteen hours to complete. These [Google](https://docs.google.com/document/d/1nOadoTU2YxaevYkYJpwsabKDq06GyWiE0W6nnG-Uf7M/edit?usp=drivesdk) [Docs](https://docs.google.com/document/d/1kyIok-TIUp33ot2DaDsc0yfSlF2Xqls6P4McMn81uI0/edit#) documents every week as it happened.

**Week 1-**
The method for completing the project was fleshed out. 54 songs were chosen from the game that had the hardest difficulty, 18 and 19. This was so there would be enough score variance between the top players. The top fourteen players from the DDR ranking website plus the third place Konami Arcade Championship finalist would be evaluated for their scores. Data will be taken from [Skill Attack](http://skillattack.com/sa4/) or Twitter, whichever one provides more accurate scores.

**Week 2-** A [Google Sheets](https://docs.google.com/spreadsheets/d/1iJwB6DM1Rgd7vcykuHsGiLuTWSulf_7CsIXnuPkISbw/edit?usp=sharing) was created to document the data.
 “Song Information” tab was created, along with most of the columns. This intends to document every attribute of a song that could possibly contribute to its difficulty.

**Week 3-**
Player data was added, which collects the scores from the fifteen top players mentioned above, plus what kind of combo they achieved. Their scores were then combined to form an average score for every song and player. Any scores left undocumented were left blank.

**Week 4-**
The “User Information” tab was added, which went over the top players and some basic information about them. This tab was largely unused. More columns were added to the Song Information tab and the player scores were finalized.

**Week 5-**
The data taken from the first two slides were combined. Each column from Song Information was lined up and compared with the average score. Two scatter plots were made per column. One with a range of 925,000-1,000,00 and one with a range of 990,000-1,000,000 to better examine the data without the inclusion of the outliers that were given a 19 difficulty. The top two easiest and hardest ranges were documented. My coworker also attempted to analyse the data using Python and the results were compared to try and find correlation.

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/code.png)

**Week 6-**
The (incomplete) findings were posted on Github with the intention to finish in the future. This was mostly learning how to use Github and how to clearly present the data in website format.

**Week 7-**
Two song files were charted and the download link was provided. Anyone can now view and play the two files via Stepmania. The stats for both of the songs can be seen [here](https://docs.google.com/spreadsheets/d/134HJ1K5NMneQ5BUBdozxQiMSxIQhdLy4YYYz-SJIV9U/edit?usp=sharing). The improvements section was added, going over ways this project could be improved.

**Week 8-**
The songs were recorded and uploaded to YouTube for viewers who can't download Stepmania. Any additional issues were fixed.

## Song Information column explanation
Song- The song’s title 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/DEGRS.png)

ID- The song’s identification number, ordered by average score of the selected fifteen players

Length (seconds)- The song’s length in seconds 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/Length.png)

Notes- The amount of arrows, or notes, a song has. Does not count jumps or shock arrows. (The leftmost number) 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/Note.png)

Freeze Arrows- Amount of hold arrows, which have a trail following them. (The middle number) 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/Note.png)

Shock Arrows- Amount of rows of shock arrows, which are not meant to be stepped on and break the player's combo when stepped. (The rightmost number) 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/Note.png)

Jumps- Amount of jumps, portrayed by two arrows hitting the receptor at the same time 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/Jump.png)

BPM- The beats per minute of the main melody of the song 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/BPM.png)

Peak BPM- Highest BPM a song reaches when at least one note is hit

Lowest BPM- Lowest BPM a song reaches when at least one note is hit

#of Stops- Number of times the stepchart stops moving. [Chaos](https://www.youtube.com/watch?v=LJIMACIMzv8) is a song known for having a lot of stops.

#BPM changes- Number of times the stepchart changes speed [Ace for Aces](https://www.youtube.com/watch?v=ujm0IFNSmA8) is a song known for having a lot of bpm changes.

Notes/Second- Number of notes divided by seconds

Year of Origin- Year the song was originally released to the game 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/Date.png)

#of Crossovers- Number of left-up-right, left-down-right, and vice versa step patterns 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/crossover.png)

Difficulty- Difficulty rating given by Konami, the game’s developer. While the normal scale is 1-20, this project focuses on songs rated 18-19. 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/DEGRS.png)

Air- Air value for a song given by Konami, used to reverse calculate jumps (obsolete since it's essentially a more confusing jump stat) 

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/Air.png)

Avg score- Average score of fifteen selected players

FArrows PS- Freeze arrows divided by seconds

JPS- Jumps divided by seconds

CPS- Crossovers divided by seconds

# Results: 
The results were calculated by eyeballing the graphs and picking ranges which stand out. Interpretations are made over whether or not the correlation equals causation in each dataset

![](https://github.com/veryprofessional/DDRData/blob/gh-pages/data.png)

**Length (seconds)**

Hard 115-125, 95-105.

Easy 105-115/125-135,	90-95

Interpretation: The first thing to point out is that Komani likes to "balance" charts in DDR. If a chart is very difficult in one aspect, other aspects are usually made less challenging to prevent making the song unapproachable. We can see this happens with the song length. Logically, a long song would be harder, since there would be more notes. However, this is not the case in DDR. Because the songs are long, they are balanced out by making the notes less dense. This in turn means that long songs usually have less NPS than their shorter counterparts and as a result are easier. 

**NPS**

Hard 7.5-8.5,	6.5-7

Easy	5-5.5	6-6.5

Interpretation: The faster a song, the more notes there are to hit. However, DDR isn't that simple. If a song has less NPS, especially if it's in the 18-19 range, the patterns are typically more complex. There are more crossovers, footswitches (patterns that make the player shift their feet position), and overall higher technicality. While a very large skill barrier, it it's effect is minimal at the top level of play, as shown here. The NPS perfectly correlaes with the difficulty once technical patterns are no longer an issue.

**FAPS**

Hard	.3-.35,	0.75

Easy	.4-.6,	.11-.35

Interpretation: There is a slight upwards trend in difficulty, but it doesn't perfectly correlate. This is likely due to the fact that freeze arrows are entirely dependent on how they are used. 

**Shock Arrows**

Hard	0,	50+

Easy	0,	1-25

Interpretation: There are only four shock arrow charts out of the fifty four analyzed songs. Konami knows how unpopular these types of charts are and therefore keep them simple and scarce.

**JPS**

Hard	.25-.4, .7-1.05

Easy	.4-.6,	0-.25

Interpretation: Jumps are usually put in a song to compensate for less notes. Either that, or they are thrown in an already fast song, which seems to be the case for the .25-.4 range.

**BPM**

Hard	220,	170-180

Easy	200-210,	180-190

Interpretation: The more extreme the BPM, the harder it is to see the notes

**Peak BPM**

Hard	700-900,	160-190

Easy	200-240,	300-450

Interpretation: Same as BPM

**Lowest BPM**

Hard	0-150,	210+

Easy	190-210,	175-185

Interpretation: Same as BPM

**#of Stops**

Hard	0,	5-10

Easy	1-5,	10-15

Interpretation: Stops, while disruptive, are easy to telegraph. There is no real correlation since stops are a non-issue once they are memorized.

**#BPM changes**

Hard	0-10,	0

Easy	10-20,	0

Interpretation: A song with too many BPM changes usually revolves around them, and suffers in other departments. The trick is to keep them scarce but significant. About half of the charts have zero BPM changes, which is why they are simultaneously the second hardest and easiest.

**Year of Origin**

Hard	2020,	2019

Easy	2016,	2006

Interpretation: In 2016, DDR A was released, the first North American DDR release in six years. Because of this, it makes sense Konami would release easier songs to get players back in the groove. The other dates make sense because more time since release = more time to practice.

**CPS**

Hard	.2-.3,	.7+

Easy	0-.2,	.3-.4

Interpretation: Crossovers are the hardest pattern in the game. It makes sense harder songs would include lots of them.

**Difficulty**

Hard	19

Easy	18

Interpretation: This is the rating Konami officially gave the songs. It looks like they did a good job.

# Conclusion: 

I made two stepfiles which showcase what it would look like if a song had the every hardest/easiest attribute, using the data from the top two results. The only exceptions are year, which is impossible to control. These charts do not factor causation to make the charts as similar to real DDR charts as possible ("balancing" the charts).

[Easy](https://drive.google.com/drive/folders/1VfXyj_KN-0wigAWfjo_2ofI5AbJyxQC7?usp=sharing)    [Youtube link](https://youtu.be/ODigGu3wJZQ)

[Hard](https://drive.google.com/drive/folders/1SazX8uGqthcrPn05KGRlU2yEdPxtJT5I?usp=sharing)    [Youtube link](https://youtu.be/rZmNcZAu6g4)

