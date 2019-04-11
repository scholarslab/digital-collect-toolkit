---
layout: default
title: Introductory Lesson on Twarc
parent: Social Media Tools
nav_order: 3
---

# Introductory Lesson on Twarc for Twitter Data Collection
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Why Collect Tweets?
Twitter is undeniably a part of the cultural landscape of the modern world, and its content represents a new form of the historical record, one that archivists around the world are actively working to preserve.

Particularly relevant to researchers interested in exploring popular movements, the dynamics of fast-moving socio-political events, and the digital footprint of contemporary culture, Twitter archiving is becoming increasingly more prominent in the catalog of activities taking place under the umbrella of digital curation.

Like other digital archiving efforts, the collection and curation of Twitter data does involve some unique challenges, not least of which is the functionally infinite size of the dataset.  For this reason, a large part of collecting, archiving, and providing access to Twitter data involves deciding what to collect and why.  Any Twitter archive will reflect the intention of its collector - from the tools used to gather the data to the kind of search used to collect, Twitter archives are always a directed slice of the ever-expanding pie that is social media.  

## Data Collection Process
The University of Virginia currently archives collections of Twitter data using [Twarc](https://github.com/DocNow/twarc), a command line tool and Python library developed as part of the [Documenting the Now](https://www.docnow.io/) project. Twarc provides several different methods for collecting Twitter data, which are outlined below. Note that each collection method has a distinct goal in mind, and will have slightly different outputs depending on how the data is collected. It is important to note the kind of collection process used to generate a specific Twitter archive - the table below outlines some of these variations and the effects on their output. The type of collection method should be noted in the description of each Twitter archive, as well as the date and size of the collection, along with the dates of collection and dataset size.

## Common Twarc Collection Methods Used in Archiving
_For more detailed usage documentation, see the following page on [Twarc Commands]({{ site.baseurl }}{% link docs/social-media/twarc-commands.md %})._
_You can also [skip ahead to the beginner's tutorial on using Twarc](#start-collecting-twarc-command-basics)._
### Search
Collects pre-existing tweets from up to seven days ago that match the given query.  This method allows you to gather tweets that are already published, but will not collect any tweets that have been made private or deleted by the time you run your search.
### Filter
Initiates a collection process that will gather tweets matching the given query as they are published.  This process does not gather tweets that were already published by the time the filter is initialized, but will ensure a high-fidelity capture of all material between the start and end times of the filter.  Unlike a search, it is also not limited to a single week, and can be run as long as you want.  
### Sample
This method returns a random sampling of tweets.
### Timeline
The timeline command will collect the most recent tweets from a single user.  Like search, it can only go back seven days.

### Side by Side: Search vs Filter
The following example illustrates some of the differences between using search and filter methods with the same arguments and output. In this case, we are looking for all tweets containing the keyword “charlottesville”.  

|| Search      | Filter |
|| ----------- | ----------- |
|**Twarc Command**| twarc search <span style="color:blue">charlottesville</span> > <span style="color:blue">charlottesville-tweets</span>.jsonl | twarc filter <span style="color:blue">charlottesville</span> > <span style="color:blue">charlottesville-tweets</span>.jsonl |
|**Description** | Searches all existing tweets from the present to seven days earlier (this time limit is set by Twitter).| Initiates a collection process that will gather tweets, as they are published, until you tell it to stop.|
|**Output** | Returns results as a JSONL file, where each JSON object = a single tweet.| Returns results as a JSONL file, where each JSON object = a single tweet.|
|**Notes** | Captures all relevant tweets up to a week prior to the search date, but will not capture any tweets that have been either privatized or deleted by the time the search is run.| A higher-fidelity collecting method that archives tweets in real time. Twarc filtering requires a dedicated machine that stays on for the duration of the process.|

_The <span style="color:blue">blue text</span> in the twarc command field is modifiable: this is where you tell Twarc what you want to search for, and where you want to name the JSONL file that will contain the results._ 
{: .fs-3 }

## Dehydrated and Rehydrated Data Sets

Twitter API's [Terms of Service](https://developer.twitter.com/en/developer-terms/policy#6._Be_a_Good_Partner_to_Twitter) does not allow for making large amounts of raw Twitter data available on the Web. The fully-hydrated Twitter data you collect using Twarc can be used for research and archived for local use, but cannot be shared publically. However, Twitter does allow files of tweet identifiers to be publically shared. This is useful for when you would like to make a dataset of tweets available, for example, in [DocNow's Tweet Catalogue](https://www.docnow.io/catalog/). This is referred to as a "dehydrated" data set - each tweet is reduced to its unique ID number, and a list of these IDs is saved as a text document. You can [use Twarc to dehydrate your data set](#dehydrate-your-dataset). 

A dehydrated data set can be ["rehydrated" using Twarc](#rehydrate-a-dataset) or another program of your choice - Twitter will take each ID and search the current Twitterverse for a corresponding tweet. If it locates a tweet that matches the ID, it will return the original JSON code for that tweet. This process is called “rehydration”, and will return a JSON file containing the data for every tweet that it was able to locate. It’s important to note that any tweet rehydrator can only check for tweets that are currently live - they cannot find tweets that have been deleted or made private since the original collection event.  

## Start Collecting: Twarc Command Basics

### Collecting Tweets
Let's start collecting tweets! This introductory lesson will use Twarc’s search command to return tweets containing ‘BlackLivesMatter’ occurring within the past 7 days. For further instructions on using other commands, see the following page on [Twarc Commands]({{ site.baseurl }}{% link docs/social-media/twarc-commands.md %}). This lesson assumes some basic familiarity with the command line (Terminal for Mac users, PowerShell for Windows users).

1. Create a new folder on your desktop titled ‘BlackLivesMatter_Tweets’.
2. Open Terminal (for Mac) or PowerShell (for Windows)
3. Change directories to navigate into the ‘BlackLivesMatter_Tweets’ folder by typing into the command line `cd` followed by the path of your folder:

        cd desktop/BlackLivesMatter_Tweets

    Hit 'return' to complete the command.

    You can also navigate to your folder by typing `cd` followed by a space, then drag your folder into the Terminal or PowerShell window. Hit return to complete the command

    To check if you are in the correct place, use the command `pwd` to display the path of your current directory. It should end with `/BlackLivesMatter_Tweets`
4. Now that you are in the right directory, enter the following command to start collecting tweets:

        twarc search blacklivesmatter > blacklivesmatter_tweets.jsonl

    _Tip: You can copy and paste these commands into Terminal or PowerShell to avoid errors_

    **Note**: Your collection may take some time to return all Tweets. You can tell when the process is complete when it returns to the shell ($) (or PowerShell (PS) ) prompt:
    
    ![Screen shot of terminal twarc search]({{ site.url }}{{ site.baseurl }}/assets/images/terminal-3.png)

    
5. While the prompt is running, check to make sure your command was successful by clicking on your ‘BlackLivesMatter_Tweets’ folder. Inside you should see your ‘blacklivesmatter_tweets.jsonl’ file and a ‘twarc.log’ file. 

    ![Screen shot of ‘BlackLivesMatter_Tweets’ folder contents]({{ site.url }}{{ site.baseurl }}/assets/images/tweet-data-folder.png)

6. For the purposes of this tutorial, you can cut the search short. After entering the initial  search command, wait 5 minutes and then enter Ctrl + C to stop the search. 

    **Note**: If you wanted to collect the full set of tweets, you would wait until the process was finished. You can tell when a process is complete when it returns to the shell ($) prompt.
7. You're done! Your tweets are in JSON format in your ‘blacklivesmatter_tweets.jsonl’ file.

### Dehydrate your Dataset

Each Tweet in your dataset has a unique identifier. Twarc’s dehydrate command will generate a list of tweet ids from a file of tweets. This lesson will show you how to dehydrate your ‘blacklivesmatter_tweets.jsonl’ file so that you can share your dataset while keeping to Twitter API's [Terms of Service](https://developer.twitter.com/en/developer-terms/policy#6._Be_a_Good_Partner_to_Twitter). 

1. Navigate into you ‘BlackLivesMatter_Tweets’ folder using the `cd` command, or if you are already there, check you directory location using the `pwd` command.

2. Enter the command `ls` to list all files in the directory. You should see the files ‘blacklivesmatter_tweets.jsonl’ and ‘twarc.log’. It will look something like this:

        'your-computer-name':BlackLivesMatter_Tweets 'your-user-name'$ ls
        blacklivesmatter_tweets.jsonl	twarc.log
3. To dehydrate your tweets, enter the following command:

        twarc dehydrate blacklivesmatter_tweets.jsonl > blacklivesmatter_tweet_ids.txt 

4. You should now have a text file containing the unique tweet ids of all tweets in your dataset. Your tweet ids are located in your ‘BlackLivesMatter_Tweets’ folder in the ‘blacklivesmatter_tweet_ids.txt’ file.

    ![Screen shot of ‘BlackLivesMatter_Tweets’ folder contents]({{ site.url }}{{ site.baseurl }}/assets/images/tweet-data-folder-2.png)

5. Open the blacklivesmatter_tweet_ids.txt file to see the list of unique tweet ids:

    ![Screen shot of txt file contents]({{ site.url }}{{ site.baseurl }}/assets/images/txt-file-ids.png)

### Rehydrate a Dataset

Twarc’s hydrate command will read your file of unique identifiers and write out the tweet JSON for them using Twitter's [status/lookup API](https://developer.twitter.com/en/docs/api-reference-index). This is useful if you have a set of Twitter ids from another institution and would like to view the full dataset. [Documenting the Now](https://www.docnow.io/) has a collection of Tweet ids that you can explore and rehydrate [here](https://www.docnow.io/catalog/), but for this tutorial we will use the ‘blacklivesmatter_tweet_ids.txt’ file you created when you dehydrated your dataset. 

1. Navigate into you ‘BlackLivesMatter_Tweets’ folder using the `cd` command, or if you are already there, check you directory location using the `pwd` command.

2. Rehydrate your dataset by entering the following command:

        twarc hydrate blacklivesmatter_tweet_ids.txt > blacklivesmatter_tweets_hydrated.jsonl 

3. You now have your tweets in JSON format ready to go in your ‘BlackLivesMatter_Tweets’ folder. Check your folder to confirm your .jsonl file is there.

Now you're ready for more complex Twarc commands that will allow you to create a collection to fit your research needs: [Twarc Commands]({{ site.baseurl }}{% link docs/social-media/twarc-commands.md %}).

