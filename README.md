This is my implementation of a solution for the following challenge:

(originally featured
[here](https://www.hackerrank.com/contests/jointheflock/challenges/identify-the-tweeter))

# Identify the Tweeter

One day you accidentally deleted the usernames, but the not the tweets. You could retrieve the data by using a backup, but decide that would be no fun. Instead you use Machine Learning to find the owner of the tweets. Luckily you only deleted the following usernames:

@justinbieber
@BillGates
@KingJames
@google
@BarackObama

## Training Data

In order to figure which tweet belongs to which owner. You pulled some of the tweets made by all five owners from the database. The file can be downloaded here, and will be included in the directory your program is run from with the name “trainingdata.txt”. The file is formatted as follows:

The first line contains an integer, n, the number of tweets that follow. The next n lines will first have the username of the owner of the tweet, followed by a space, then the tweet itself.

## Input

The first line will contain an integer t, the number of tweets who have lost their owner. The next t lines will each contain a tweet (up to 140 characters)

## Output

Output who you think the owner of each tweet is on its own line. Do not include the @.

## Sample Input

5

Tell Congress: #NowIsTheTime to close background check loopholes for gun sales. http://t.co/PiAdjEbV, http://t.co/rmcJKN6H

Today the #BELIEVEtour hits New Jersey and I am proud that we will donate a portion of ALL tix sold to Hurricane Sandy Relief. #GIVEBACK

What does Ronald McDonald and @DwyaneWade have in common? They both 6’2 and wear size 20 shoe!!

PHOTOS: My trip to Ghana where I saw what is working & what can be shared with other countries http://t.co/qMYIMsQCYN http://t.co/eRssXUzY6r

Jewish Googlers lit up their not-so-traditional, but very googley, lava lamp menorah last night. Happy Chanukah! http://t.co/cEPwS1vo

## Sample Output

BarackObama

justinbieber

KingJames

BillGates

google

## Scoring

Your score for this challenge will be 60 * ( 4 * # correctly classified tweets - # of incorrectly classified tweets)/ (4 * total # of tweets) 
