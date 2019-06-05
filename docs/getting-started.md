---
layout: page
title: Getting Started
permalink: /docs/site-building/
nav_order: 1
---

# Getting Started
{: .no_toc }
The basics for building a rapid response Digital Collection Site
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Gathering a Team

In order for your digital collecting strategies to be successful, you may need to gather experts from across your organization.  Here are some areas of expertise and types of responsibilities those team members might have:
-	**Project lead**
    - Coordinate team, set up meetings and deadlines, document outcomes
-	**Metadata**
    - Determine how content should be structured for ease of submission and description, future use/reuse
    - Describe/remediate description of content
-	**Preservation**
    - Ensure short and long-term access to content
    - Select appropriate tools for ingest and preservation
-	**Legal counsel**
    - Protect organization 
    - Ensure institution can preserve and provide access over time
    - Consider implications of collecting on donors, people being documented
-	**IT specialists and content developers**
    - Consider security, server capacity, and storage
    - Install and configure Omeka, select templates/plug-ins and tools for capture
-	**Communications and user experience**
    - Review language and layout for ease of use by non-specialists
    - Documentation for internal and external users
-	**Outreach**
    - Liaison to community from whom you are trying to collect
-	**Collections specialist**
    - Define the scope of the digital collection (types of materials, collection duration)
    - This might come from your special collections or other subject area

## Ethical Considerations

Implementing and maintaining a digital collection site requires ethical, community-centric practices. We've compiled some sources that explore these considerations, and strongly encourage anyone developing an archive from community contributions and/or social media content to read further:

-	Michelle Caswell, [“Toward a Survivor-Centered Approach to Human Rights Archives: Lessons from Community-Based Archives.”](https://link.springer.com/article/10.1007/s10502-014-9220-6) Archival Science 14: 3-4 (2014): 307-322.
- GWU Libraries' Social Feed Manager (SFM), [Building Social Media Archives: Collection Development Guidelines](https://gwu-libraries.github.io/sfm-ui/resources/guidelines)
- [An Invitation Towards Social Justice in the Digital Humanities](http://criticaldh.roopikarisam.com/)
- [Anti-oppression principles compiled by the Center for Story-Based Strategy](https://www.storybasedstrategy.org/anti-oppression-principles)

## Funding Opportunities

This project was made possible in part by a 2018 award from the [Catalyst Fund at LYRASIS](https://www.lyrasis.org/Leadership/Pages/Catalyst-Fund.aspx). It may be worth exploring grant programs that can help support your digital collections.

[Documenting the Now](https://www.docnow.io/) has an annual call for applicants for Community-Based Digital Archives Workshops for Activists. Their workshops focus on helping activists to develop the skills and to use available tools to collect, preserve, and share their web, social media and other types of digital content in their own digital archive.

## Technical Considerations

### Omeka for Digital Collections

Omeka offers two platforms -  Omeka Classic and Omeka S - for publishing and managing your digital collections. Our digital collecting site runs on [Omeka Classic](https://omeka.org/classic/){:target="_blank"}, which is at the core of what is currently offered in this toolkit. Follow the materials in our toolkit section on [Setting up Omeka Classic]({{ site.baseurl }}{% link docs/omeka-setup/custom-theme.md %}) to build a site similar to [_"Unite the Right" Rally and Community Response_](http://digitalcollecting.lib.virginia.edu/rally/){:target="_blank"}. We've identified [plugins]({{ site.baseurl }}{% link docs/omeka-setup/omeka-plugins.md %}) and created a [custom theme]({{ site.baseurl }}{% link docs/omeka-setup/custom-theme.md %}) specifically for use with Omeka Classic. 

Your project needs may align instead with [Omeka S](https://omeka.org/s/){:target="_blank"}, which offers many of the same options as Omeka Classic. Instead of plugins, Omeka S provides [modules](https://omeka.org/s/modules/){:target="_blank"} to extend the functionality of your site. The [Collecting](https://omeka.org/s/modules/Collecting/){:target="_blank"} module offers the equivalent to the Contribution plugin for collecting public contributions through your site. The [Custom Vocab](https://omeka.org/s/modules/CustomVocab/){:target="_blank"} module is comparable to the Simple Vocab plugin for providing predetermined vocabulary for any metadata elements. See the complete [User Manual](https://omeka.org/s/docs/user-manual/){:target="_blank"} for Omeka S, and the complete list of [modules](https://omeka.org/s/modules/){:target="_blank"} for that platform.


### File Size Limitations

You'll want to consider setting a limit on the file size for individual contributions uploaded through your site's collection form. These settings are server specific, and can be set up by your server administrator when you install Omeka. If you're using Reclaim Hosting, or another shared hosting service, you may not be able to change the file size limitations. 

For our digital collecting site, we set the maximum file size for uploads at 250Mb. This is large enough for short video files taken with smartphones, which was an item we were interested in collecting. Creating a limit on file size may seem restrictive, but it is important for the sustainability of your server, where your files are stored. Your available server space is determined by your institution or your shared hosting service (like [Reclaim](https://reclaimhosting.com/){:target="_blank"}), so consider how much total space you have for file storage when determining size restrictions. 

### Large Files and File Sets

Currently, the Contribution plugin for Omeka Classic allows for only individual file uploads, with a maximum file size set by your server administrator. For our site, we encourage contributors to use the contribution form to submit their materials, as it provides the simplest way for us to process the items we receive. However, for files larger than 250Mb or for large file sets we provide an option for contributing a URL link for an album or file location (i.e. Dropbox folder, Flickr album, etc.). When images and video files are uploaded directly through the contribution form, they're processed as Omeka items, and easily managed from the Omeka dashboard. Materials submitted as links have required significantly more time on our end to include them in the collection, and has been a major impediment to making more of our archive public. 

Omeka offers the Dropbox plugin, which lets Omeka users batch upload a large quantity of files at once. It allows you to upload multiple files directly into a folder on your server that you can then add in the items admin interface. We have not used this plugin at this time for our site, but it offers one option for handling large file set submissions.

- [Dropbox plugin download](https://omeka.org/classic/plugins/Dropbox/){:target="_blank"}
- [Dropbox plugin User Guide](https://omeka.org/classic/docs/Plugins/Dropbox/){:target="_blank"}


This page was published: April 25, 2019
{: .fs-3 }
