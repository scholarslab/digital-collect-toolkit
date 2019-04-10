---
layout: default
title: Install & Configure Twarc
parent: Social Media Tools
nav_order: 2
---
# Installing and Configuring Twarc
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Before you Begin

1. Before using [Twarc](https://github.com/DocNow/twarc), you will need to [register a Twitter application](../social-media/twitter-setup), and have your [consumer key, consumer secret, access token, and access token secret](../social-media/twitter-setup#accessing-keys-and-tokens) on hand. 

2. Twarc requires familiarity with using the command line to navigate your file system, configure Twarc, and run queries. For introductory lessons on using the command line, see these tutorials for Mac and Windows users from the UNLV Libraries, [here](https://www.library.unlv.edu/whats_new_in_special_collections/2019/02/new-digital-collections-introduction-command-line.html). 
   
   The Command Line tutorial is part of UNLV Libraries' [Twitter Data Tutorial Series](https://www.library.unlv.edu/whats_new_in_special_collections/2019/04/new-digital-collections-1-october-twitter-data-tutorial), which features ten tutorials that take you step-by-step through the design, collection, and documentation process of curating a collection of Twitter data, as well as tutorials on tools for data analysis. This series is focused on using Twarc and offers another resource, in addition to this toolkit. 

3. Download and install the latest version of Python, [here](https://www.python.org/downloads/). Twarc works with with either version 2 or 3.

   If you are a Mac user, you may already have Python installed. To check, open your terminal and run the command:

   `python -V`

   or

   `python --version`

## Twarc for Mac OS
_For Windows users, click [here](#twarc-for-windows)_

### Installing Twarc

1. Open the Terminal application (located in the applications folder)
2. Pip install Twarc by entering the following command: 

   `pip install twarc`

   _Note: [Pip](https://pip.pypa.io/en/stable/installing/) is already installed if you are using Python 2 ≥ 2.7.9 or Python 3 ≥ 3.4_

   macOS users also have the option of installing Twarc via homebrew using the command:

   `brew install twarc`

### Configuring Twarc

To get started, you will need to tell Twarc about your application API keys and grant access to one or more Twitter accounts. Follow these directions to configure Twarc:

1. Enter the following command in Terminal:

   `twarc configure`
2. Twarc will ask you to enter several keys. You should have these keys ready to go after [registering an application](../social-media/twitter-setup#accessing-keys-and-tokens). 

   ![Screen shot of Terminal]({{ site.url }}{{ site.baseurl }}/assets/images/terminal-1.png)

   Type or copy/paste your consumer key, then press 'enter'. Next, Twarc will ask for your consumer secret. Type or copy/paste your consumer secret, then press 'enter'.
3. Next, Twarc will ask you to log into your twitter account. Copy/paste the provided URL into your browser to authorize your application. 

   ![Screen shot of twarc request]({{ site.url }}{{ site.baseurl }}/assets/images/terminal-2.png)

4. Following the provided URL will bring you to a page that looks something like this:

   ![Screen shot of twitter authorize page]({{ site.url }}{{ site.baseurl }}/assets/images/twitter-authorize.png)

   Click 'Authorize app'. A pin number will be provided, Type this pin into your terminal, as seen in step 3, then press 'enter'.

5. After entering your pin, your terminal should give a message telling you where your twitter credentials are saved, followed by "Happy twarcing!" This means your twarc installation is configured and you can now start [collecting tweets](../social-media/collect-tweets)!

## Twarc for Windows

### Installing Twarc

1. Open PowerShell (to open PowerShell, use the taskbar to search for PowerShell and select ‘Windows PowerShell’)
2. Pip install Twarc by entering the following command: 

   `pip install twarc`

   _Note: [Pip](https://pip.pypa.io/en/stable/installing/) is already installed if you are using Python 2 ≥ 2.7.9 or Python 3 ≥ 3.4_

### Configuring Twarc

To get started, you will need to tell Twarc about your application API keys and grant access to one or more Twitter accounts. Follow these directions to configure Twarc:

1. Enter the following command in PowerShell:

   `twarc configure`
2. Twarc will ask you to enter several keys. You should have these keys ready to go after [registering an application](../social-media/twitter-setup#accessing-keys-and-tokens). 

    Type or copy/paste your consumer key, then press 'enter'. Next, Twarc will ask for your consumer secret. Type or copy/paste your consumer secret, then press 'enter'.
