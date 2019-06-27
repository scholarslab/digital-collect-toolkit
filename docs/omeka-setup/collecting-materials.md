---
layout: default
title: Collecting Community Contributions
parent: Omeka Classic Setup
nav_order: 2
---

# Collecting Community Contributions
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

It is important to make clear in your Terms of Service that user anonymity is conditional, and it is likely that under a lawful subpoena or court order, all submissions and associated data may be required to be provided to federal, state, or local law enforcement or other government agencies. See our [Terms of Service](#contribution-terms-of-service) section for more details. 

For further documentation on Contribution Submission Settings and Contributor anonymity settings, see the related [Omeka Documentation](https://omeka.org/classic/docs/Plugins/Contribution/#submission-settings).

## Contribution Terms of Service

We offer a general Contribution Terms of Service template for others as a model. [Our terms](http://digitalcollecting.lib.virginia.edu/rally/contribution/terms) were written in collaboration with University of Virginia General Council. We recommend reviewing your terms with relevant parties for your own collecting site. 

>**Contribution Terms of Service:**

>You are being asked to contribute your recollections, photographic images, video, social media postings or other digital content to [insert institution here], which is creating a digital record of the [describe event, location, and date(s) here]. 
{: .fs-4 .fw-300 }
>You may only submit material created entirely by you and not copied from or based, in whole or in part, upon any other photographic, literary, or other material, except to the extent that such material is in the public domain, or you have permission of the copyright owner, or its use is allowed by "Fair Use" as prescribed by the terms of United States copyright law.  If you would like to refer or nominate material which you do not own, please contact us at [insert email address or link to google nominating form].
{: .fs-4 .fw-300 }
>You must be 18 years of age or older to submit material. By submitting content through this form, you are granting [insert institution here] permission to disseminate, preserve, and use that content in connection with its educational and research mission, including promotional purposes, in all media in perpetuity.   You retain ownership of and copyright in the material you share. 
{: .fs-4 .fw-300 }
>If you indicate on the form that your submission is “public,” your material may be published on the web (with or without your name, depending on what you have indicated) as part of [insert institution here] digital collections or exhibits. Otherwise, your material will only be available to [insert institution here]-approved researchers.  
{: .fs-4 .fw-300 }
>Submitted material must not violate any confidentiality, privacy, security or other laws. Please be aware that all submissions and any information associated with the submissions (email address, descriptive information, etc.) may be provided to federal, state, or local law enforcement or other government agencies pursuant to a lawful subpoena or otherwise as required by law. 
{: .fs-4 .fw-300 }
>We reserve the right to discard or mark private any submission that [institution] staff identify as irrelevant or for any other reason within their professional judgment. [Insert institution here] is not obligated to include your content in this project or preserve it in perpetuity.
{: .fs-4 .fw-300 }

In addition, our Digital Collecting site's [Terms of Service](http://digitalcollecting.lib.virginia.edu/rally/contribution/terms) includes a Summary of Terms to help contributors quickly read and understand the main points of the full terms, in simpler language. It is important to note to users that a summary does not replace the full terms, and submissions are governed by the full terms of use.

>**Summary of Terms***

> - You must be at least 18 years old.
> - Submitted material must be owned and/or created by you.
> - You have the option of making your contribution public or private. If public, your content may be published as part of the Library’s digital collections (with or without your name displayed, depending on what you have indicated).
> - All submissions will be available to Library-approved researchers and can be used by the Library from now on in support of its teaching and research mission.
> - Your submission must not violate any laws. If we receive a lawful subpoena or court order, we may be required to turn over any submissions and related information (email address, descriptive information, etc.).
{: .fs-4 .fw-300 }
>*This summary is to help you read and understand the terms, but does not replace them. Your submission is governed by the full terms of use.
{: .fs-4 .fw-300 }