---
layout: default
title: Setting up the Contribution plugin
parent: Omeka Classic Setup
nav_order: 2
---

# Setting up the Contribution plugin
{: .no_toc }

We've included detailed documentation on how our [Digital Collecting](http://digitalcollecting.lib.virginia.edu/rally/) site uses the [Contribution plugin](https://omeka.org/classic/plugins/Contribution/) for Omeka to collect stories, images, videos, and links from the public. 
{: .fs-6 .fw-300 }
Please read through the plugin's [Installation & Configuration Guide](https://omeka.org/classic/docs/Plugins/Contribution/) for full set-up instructions before getting started. 
{: .fs-6 .fw-300 }

Published: April 25, 2019
{: .fs-3 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## What to Collect

Using the Omeka Contribution plugin, you can collect a wide variety of materials from the public through a content submission form on your site. You can update your plugin settings and Contribution Types at any time, but it is good to consider what content your are interested in collecting when first setting up your site. Contributions are private by default and require a site administrator to review and make them public on your Omeka site. 

Our site collects stories, photos/scanned images, videos and website links - each of these corresponding to an [Omeka Item Type](https://omeka.org/classic/docs/Content/Item_Types/): Text, Still Image, Moving Image, and Hyperlink. You have the option to allow for file uploads via the public contribution form for each Contribution Type. The list of allowed extensions for file uploads can be found in your Omeka site's [Security Settings](https://omeka.org/classic/docs/Admin/Settings/Security_Settings/). The default list contains the most common image, video, and document file extensions - including doc, docx, jpeg, png, tiff, mp3, mov, etc - so you likely do not need to make any adjustment to these settings. 

The public contribution form can provide a simple way to collect material from social media by encouraging community members to upload screenshot images, or text copied directly from a social media post. For example, our site has collected stories that were originally posted on Facebook and uploaded through the content submission form as plain text and document files. For a more advanced technical method of collecting data from Twitter, see the section on [Social Media Tools]({{ site.url }}{{ site.baseurl }}/docs/social-media).

## Creating Contribution Types

After installing the plugin, find the settings for Contribution by clicking on the "Contributed Items" tab on the left-hand navigation panel of the Omeka admin dashboard. Here you will see four tabs: Getting Started, Contribution Types, Submission Settings, and Contributions. 

Select "Contribution Types" to manage the types of items you'd like users to share through the form:

![Screenshot of Contribution Types Admin](https://raw.githubusercontent.com/scholarslab/digital-collect-toolkit/master/assets/images/contribution-types.png)

See in the above image that we have included four contribution types for our site: _Story, Photograph, Link,_ and _Video_. The type's _Name_ is the label that will appear in your site's Contribution Form:

![Screenshot of Contribution Form, Select Type](https://raw.githubusercontent.com/scholarslab/digital-collect-toolkit/master/assets/images/form-type.png)

The _Item Type_ is the type of object associated with your Contribution Type, and is selected when you add a new contribution type to your form (see the green button 'Add a Type' on the right). These are not visible to the public, but can help in defining search fields. 

Omeka comes with pre-defined item types, found by clicking on the "Item Types" tab on the left-hand navigation panel of the Omeka admin dashboard. You can edit and add to this list if needed (see the related [Omeka Documentation](https://omeka.org/classic/docs/Content/Item_Types/)). Our site uses the pre-defined types: _Text, Still Image, Hyperlink,_ and _Moving Image_.

## Contributor Anonymity Settings

Under the tab for "Submission Settings" you can set options for contributor anonymity. Our site allows both Non-Registered Contributions and Anonymous Contributions:

![Screenshot of Contribution Settings panel](https://raw.githubusercontent.com/scholarslab/digital-collect-toolkit/master/assets/images/contrib-settings.png)

It is important to make clear in your Terms of Service that user anonymity is conditional, and it is likely that under a lawful subpoena or court order, all submissions and associated data may be required to be provided to federal, state, or local law enforcement or other government agencies. See our [Terms of Service]({{ site.url }}{{ site.baseurl }}/docs/collecting-materials) section for more details. 

For further documentation on Contribution Submission Settings and Contributor anonymity settings, see the related [Omeka Documentation](https://omeka.org/classic/docs/Plugins/Contribution/#submission-settings).