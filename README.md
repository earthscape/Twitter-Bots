# Twitter-Bots-Trolls-Retweeters

------------------------------------------------  
BOTS - twitter-bots-uids.csv  
------------------------------------------------  

List of known bots for mobility research.  
Seeks to omit any human-operated account (trolls and retweeters) that actually travels.  

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


Could be added:  
Star Wars Bots  
https://arxiv.org/pdf/1701.02405.pdf  

Bursty Bot  
https://pdfs.semanticscholar.org/8240/c8f3d532eefe6826f25da0d087c6115e9325.pdf  

Juan Echeverria  
Department of Computer Science  
University College London (UCL), United Kingdom  
j.guzman.11@ucl.ac.uk (using this one first, from Bursty Bot paper)  
J.EcheverriaGuzman@ucl.ac.uk  


------------------------------------------------
TROLLS - twitter-trolls-uids.csv
------------------------------------------------

List of known trolls

ROWS 1 to 454

Russian Troll Source:
external_user_id_rounding_fixes_from_hpsci_nov17.csv


------------------------------------------------
RETWEETERS - twitter-retweeters-uids.csv
------------------------------------------------

These may contain human-operated accounts.  

ROWS 1 to 991  

social spambots #1 - retweeters of an Italian political candidate 2012  


cresci-2017.csv/datasets_full.csv/tweets.csv  

Source  
http://papers.www2017.com.au.s3-website-ap-southeast-2.amazonaws.com/companion/p963.pdf  

Other data not used in our Twitter-Bot list since it could contain human-operated accounts.  

  genuine accounts 			verified accounts that are human-operated 3,474 8,377,522 2011 3.1, 3.2  
R social spambots #1 		retweeters of an Italian political candidate 991 1,610,176 2012 3.1, 3.2  
  social spambots #2 		spammers of paid apps for mobile devices 3,457 428,542 2014 3.1, 3.2  
  social spambots #3 		spammers of products on sale at Amazon.com 464 1,418,626 2011 3.1, 3.2  
  traditional spambots #1 	training set of spammers used by Yang et al. in [44] 1,000 145,094 2009 3.1  
  traditional spambots #2 	spammers of scam URLs 100 74,957 2014 3.1  
B traditional spambots #3 	automated accounts spamming job offers 433 5,794,931 2013 3.2  
B traditional spambots #4 	another group of automated accounts spamming job offers 1,128 133,311 2009 3.2  
  fake followers 			simple accounts that inflate the number of followers of another account  


