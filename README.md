# Twitter-Bots

------------------------------------------------  
BOTS 
------------------------------------------------  

[List of bots](twitter-bots-uids.csv) - Contains 24,580 rows with 24,578 distinct users.  

----------------  
ROWS 1 to 22223  

cavarerlee-2011 (social_honeypot)  
22,223 content_polluters created from 2006 to 2010.  
Paper: Seven Months with the Devils: A Long-Term Study of Content Polluters on Twitter. Citation:  

K. Lee, B. Eoff, and J. Caverlee. Seven Months with the Devils: A
Long-Term Study of Content Polluters on Twitter. In Proceeding of the 5th International AAAI Conference on Weblogs and Social Media (ICWSM), Barcelona, July 2011. (Bibtex)  

Source:  
https://botometer.iuni.iu.edu/bot-repository/datasets.html  
“content polluters.txt” contains content polluters’ profile information in the form of “UserID\tCreatedAt\tCollectedAt\tNumerOfFollowings \tNumberOfFollowers \tNumberOfTweets\tLengthOfScreenName\t LengthOfDescriptionInUserProfile”.  

----------------  
ROWS 22224 to 23049  

varol-2017 contains a list of UIDs and a bianary in a .dat file. (Opens as a text file.)  
bot=1 and human=0  

varol-2017 is the basis for the initial training of 
BotOrNot renamed to Botometer, which uses RapidAPI for pro version  

Source:  
https://botometer.iuni.iu.edu/bot-repository/datasets.html  

Online Human-Bot Interactions: Detection, Estimation, and Characterization  
https://arxiv.org/abs/1703.03107  
Findings suggest that 9% to 15% of active Twitter accounts are bots.  

https://rapidapi.com  


----------------  
ROWS 23050 to 23452  


cresci-2017 - traditional spambots #3 - automated accounts spamming job offers  

----------------  
ROWS 23453 to 24580  

cresci-2017 - traditional spambots #4 - another group of automated accounts spamming job offers  

---------------- 

Could be added:  
Star Wars Bots  
https://arxiv.org/pdf/1701.02405.pdf  

Bursty Bot  
https://pdfs.semanticscholar.org/8240/c8f3d532eefe6826f25da0d087c6115e9325.pdf  
Wrote:
Juan Echeverria  
Department of Computer Science  
University College London (UCL), United Kingdom  
j.guzman.11@ucl.ac.uk (using this one first, from Bursty Bot paper)  
J.EcheverriaGuzman@ucl.ac.uk  


------------------------------------------------
TROLLS
------------------------------------------------

[List of trolls](twitter-trolls-uids.csv) - Contains 454 rows  

ROWS 1 to 454

Russian Troll Source:
https://github.com/fivethirtyeight/russian-troll-tweets
https://github.com/fivethirtyeight/russian-troll-tweets/files/2278803/external_author_id_rounding_fixes.zip


------------------------------------------------

SQL for mobility study data:  

SELECT count(*) total, (SELECT count(*) FROM (SELECT DISTINCT twitter_uid FROM twitter_bots_uids)x) AS distinctTotal FROM twitter_bots_uids;

SELECT all_33day.* FROM all_33day JOIN twitter_bots_uids ON all_33day.twitter_uid = twitter_bots_uids.twitter_uid

In 16 storm impacts, 34 known-bot uids were found, having produced 8,601 geotagged tweets.

Unique bots in storm data - 34
SELECT DISTINCT all_33day.twitter_uid FROM all_33day JOIN twitter_bots_uids ON all_33day.twitter_uid = twitter_bots_uids.twitter_uid

Unique bots in ph2013_tacloban_33day - none
SELECT DISTINCT ph2013_tacloban_33day.twitter_uid FROM ph2013_tacloban_33day JOIN twitter_bots_uids ON ph2013_tacloban_33day.twitter_uid = twitter_bots_uids.twitter_uid

