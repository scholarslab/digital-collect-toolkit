---
layout: default
title: Twarc Commands
parent: Social Media Tools
nav_order: 4
---

# Twarc Commands
{: .no_toc }

After you've become familiar with the basics of using Twarc to perform a search command to collect Twitter data, dehydrate an existing dataset, and hydrate a list of unique Tweet ids, you can move on to more complex commands to tailor your search to your research needs. 

Below you will find a list of commands that will allow you to create a more targeted collection. This documentation is from the [Twarc Usage Guide](https://github.com/DocNow/twarc#usage). 

Published: April 25, 2019
{: .fs-3 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### Search

This uses Twitter's [search/tweets](https://dev.twitter.com/rest/reference/get/search/tweets) to download *pre-existing* tweets matching a given query.

    twarc search blacklivesmatter > tweets.jsonl

It's important to note that `search` will return tweets that are found within a
7 day window that Twitter's search API imposes. If this seems like a small
window, it is, but you may be interested in collecting tweets as they happen
using the `filter` and `sample` commands below.

The best way to get familiar with Twitter's search syntax is to experiment with
[Twitter's Advanced Search](https://twitter.com/search-advanced) and copy and
pasting the resulting query from the search box. For example here is a more
complicated query that searches for tweets containing either the
\#blacklivesmatter or #blm hashtags that were sent to deray.

    twarc search '#blacklivesmatter OR #blm to:deray' > tweets.jsonl

Twitter attempts to code the language of a tweet, and you can limit your search
to a particular language if you want:

    twarc search '#blacklivesmatter' --lang fr > tweets.jsonl

You can also search for tweets with a given location, for example tweets
mentioning *blacklivesmatter* that are 1 mile from the center of Ferguson,
Missouri:

    twarc search blacklivesmatter --geocode 38.7442,-90.3054,1mi > tweets.jsonl

If a search query isn't supplied when using `--geocode` you will get all tweets
relevant for that location and radius:

    twarc search --geocode 38.7442,-90.3054,1mi > tweets.jsonl

### Filter

The `filter` command will use Twitter's [statuses/filter](https://dev.twitter.com/streaming/reference/post/statuses/filter) API to collect tweets as they happen.

    twarc filter blacklivesmatter,blm > tweets.jsonl

Please note that the syntax for the Twitter's track queries is slightly
different than what queries in their search API. So please consult the
documentation on how best to express the filter option you are using.

Use the `follow` command line argument if you would like to collect tweets from
a given user id as they happen. This includes retweets. For example this will
collect tweets and retweets from CNN:

    twarc filter --follow 759251 > tweets.jsonl

You can also collect tweets using a bounding box. Note: the leading dash needs
to be escaped in the bounding box or else it will be interpreted as a command
line argument!

    twarc filter --locations "\-74,40,-73,41" > tweets.jsonl


If you combine options they are OR'ed together. For example this will collect
tweets that use the blacklivesmatter or blm hashtags and also tweets from user
CNN:

    twarc filter blacklivesmatter,blm --follow 759251 > tweets.jsonl

### Sample

Use the `sample` command to listen to Twitter's [statuses/sample](https://dev.twitter.com/streaming/reference/get/statuses/sample) API for a "random" sample of recent public statuses.

    twarc sample > tweets.jsonl

### Dehydrate

The `dehydrate` command generates an id list from a file of tweets:

    twarc dehydrate tweets.jsonl > tweet-ids.txt

### Hydrate

Twarc's `hydrate` command will read a file of tweet identifiers and write out the tweet JSON for them using Twitter's [status/lookup](https://dev.twitter.com/rest/reference/get/statuses/lookup) API.

    twarc hydrate ids.txt > tweets.jsonl

Twitter API's [Terms of Service](https://dev.twitter.com/overview/terms/policy#6._Be_a_Good_Partner_to_Twitter) discourage people from making large amounts of raw Twitter data available on the Web.  The data can be used for research and archived for local use, but not shared with the world. Twitter does allow files of tweet identifiers to be shared, which can be useful when you would like to make a dataset of tweets available.  You can then use Twitter's API to *hydrate* the data, or to retrieve the full JSON for each identifier. This is particularly important for [verification](https://en.wikipedia.org/wiki/Reproducibility) of social media research.

### Users

The `users` command will return User metadata for the given screen names.

    twarc users deray,Nettaaaaaaaa > users.jsonl

You can also give it user ids:

    twarc users 1232134,1413213 > users.jsonl

If you want you can also use a file of user ids, which can be useful if you are
using the `followers` and `friends` commands below:

    twarc users ids.txt > users.jsonl

### Followers

The `followers` command  will use Twitter's [follower id API](https://dev.twitter.com/rest/reference/get/followers/ids) to collect the follower user ids for exactly one user screen name per request as specified as an argument:

    twarc followers deray > follower_ids.txt

The result will include exactly one user id per line. The response order is
reverse chronological, or most recent followers first.

### Friends

Like the `followers` command, the `friends` command will use Twitter's [friend id API](https://dev.twitter.com/rest/reference/get/friends/ids) to collect the friend user ids for exactly one user screen name per request as specified as an argument:

    twarc friends deray > friend_ids.txt

### Trends

The `trends` command lets you retrieve information from Twitter's API about trending hashtags. You need to supply a [Where On Earth](http://developer.yahoo.com/geo/geoplanet/) identifier (`woeid`) to indicate what trends you are interested in. For example here's how you can get the current trends for St Louis:

    twarc trends 2486982

Using a `woeid` of 1 will return trends for the entire planet:

    twarc trends 1

If you aren't sure what to use as a `woeid` just omit it and you will get a list
of all the places for which Twitter tracks trends:

    twarc trends

If you have a geo-location you can use it instead of the `woedid`.

    twarc trends 39.9062,-79.4679

Behind the scenes twarc will lookup the location using Twitter's [trends/closest](https://dev.twitter.com/rest/reference/get/trends/closest) API to find the nearest `woeid`.

### Timeline

The `timeline` command will use Twitter's [user timeline API](https://dev.twitter.com/rest/reference/get/statuses/user_timeline) to collect the most recent tweets posted by the user indicated by screen_name.

    twarc timeline deray > tweets.jsonl

You can also look up users using a user id:

    twarc timeline 12345 > tweets.jsonl

### Retweets

You can get retweets for a given tweet id like so:

    twarc retweets 824077910927691778 > retweets.jsonl

### Replies

Unfortunately Twitter's API does not currently support getting replies to a
tweet. So twarc approximates it by using the search API. Since the search API
does not support getting tweets older than a week twarc can only get all the
replies to a tweet that have been sent in the last week.

If you want to get the replies to a given tweet you can:

    twarc replies 824077910927691778 > replies.jsonl

Using the `--recursive` option will also fetch replies to the replies as well as
quotes.  This can take a long time to complete for a large thread because of
rate limiting by the search API.

    twarc replies 824077910927691778 --recursive

### Lists

To get the users that are on a list you can use the list URL with the
`listmembers` command:

    twarc listmembers https://twitter.com/edsu/lists/bots
