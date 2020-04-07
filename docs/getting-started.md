---
layout: page
title: Getting Started
nav_order: 1
---

# Getting Started
{: .no_toc }
The basics for preparing for a rapid response digital collecting event and building a digital collection site.
{: .fs-6 .fw-300 }

Below are some steps that you can take to prepare for an emergency event that requires a plan for digital collecting.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Gathering a Team

In order for your digital collecting strategies to be successful, you may need to gather experts from across your organization.  Here are some areas of expertise and types of responsibilities those team members might have:

-   **Project lead**
    -   Coordinate team, set up meetings and deadlines, document outcomes
-	**Metadata**
    -   Determine how content should be structured for ease of submission and description, future use/reuse
    -   Describe/remediate description of content
-   **Preservation**
    -   Ensure short and long-term access to content
    -   Select appropriate tools for ingest and preservation
-	**Legal counsel**
    -   Protect organization 
    -   Ensure institution can preserve and provide access over time
    -   Consider implications of collecting on donors, people being documented
-	**IT specialists and digital content developers**
    -   Consider security, server capacity, and storage
    -   Install and configure Omeka, select templates/plug-ins and tools for capture
-	**Communications and user experience**
    -   Review language and layout for ease of use by non-specialists
    -   Documentation for internal and external users
-	**Outreach**
    -   Liaison to community from whom you are trying to collect
-	**Collections specialist**
    -   Define the scope of the digital collection (types of materials, collection duration)
    -   This might come from your special collections or other subject area

## Policy Review

Review your institution's policies and workflows to see if current policy includes practices for digital collecting or emergency digital collecting. If possible, create or update collection policies in advance of an emergency collecting event that address digital content, social media and web archiving. You may find it useful for your organization to implement a policy specifically covering digital collecting in times of crisis that can determine when and how to initiate emergency collecting workflows and procedures.  

## Determine the Scope

Defining the scope of what you plan to collect is important for providing an efficient and sustainable response to crises and other rapidly-evolving events. Below are some questions to consider as you plan your digital collecting initiative:

- What is the purpose of collecting? What or who are you collecting for?
    - To provide the community a place to mourn/commemorate/heal?
    - To create resource for future scholars and researchers?
    - To relate to your organization's current collecting priorities?
- What is the long-term plan for collection and access?
    - How long will you be collecting digital content?
- Are there geographic boundaries for your collection?
- What perspectives are you collecting?
    - National vs local news?
    - Media outlets vs individual stories?
- How much are you attempting to collect?
    - Everything or a representative sample?

In the case of an emergency digital collecting response, you may not know at first what you need or want to collect. Collecting everything may not be sustainable long-term, and you may need to re-address your collection due to your institution's storage capacity. If so, how will you decide what to save?

In the book chapter, ["Response to the Unthinkable: Collecting and Archiving Condolence and Temporary Memorial Materials following Public Tragedies,"](https://trace.tennessee.edu/utk_libpub/15/) Ashley R. Maynor addresses some selection criteria used by Virginia Tech in the wake of the April 16, 2007 school shooting. To determine what physical materials to keep, the school consulted with various experts, including staff from the Library of Congress. Below is a list of some selection criteria that may be relevant to your digital collection strategy:

- Popular culture
- Sociological interest
- Personal messages to victims/perpetrator
- Help personalize the lives that were lost
- Student and community groups
- Weird or unusual items
- Particularly beautiful materials
- From folks with connection to institution/community
- Unique and special material
- Official responses from government
- Representing different perspectives



## Assess your Resources

Your resources may determine or limit the scope of your emergency response digital collecting initiative. Consider team member's available time and impact to other workflows and projects. Determine your staffing needs in relation to the scale of your emergency digital collecting, as well as available funding that can help support the work. Creating a digital archive requires storage space, assess your needs in supporting short and long-term collection, as well as future access to materials. 

Given the sensitive nature of events that require an emergency digital collecting response, do not underestimate the immediate and long-term emotional impact of the work. Have a plan in place to support people working on your collection if it involves difficult content, and take breaks when needed. 

## Ethical Considerations

Implementing and maintaining a digital collection site requires ethical, community-centric practices. Issues like lack of informed consent and privacy, potential for harm, and censoring or restricting content are some of the ethical issues to consider. 

For our community collection site, we included a Statement of Values on our homepage with a link to the [Society of American Archivists’ commitment to ensuring the diversity of archivists](https://www2.archivists.org/advocacy/diversity-and-inclusion-initiatives), to emphasize our desire for all perspectives and to be as inclusive as possible when gathering materials. We developed a [Terms of Service]({{ site.url }}{{ site.baseurl }}/docs/collecting-materials) in collaboration with University of Virginia General Council, and also provided users with a [Summary of Terms]({{ site.url }}{{ site.baseurl }}/docs/collecting-materials) to help contributors quickly read and understand the main points of the full terms, in simpler language.

We've compiled some resources that explore these ethical considerations, and strongly encourage anyone developing an archive from community contributions and/or social media content to read further. You can find our reading list in the [Additional Resources]({{ site.url }}{{ site.baseurl }}/docs/additional-resources).

## Technical Considerations

This toolkit currently provides documentation on setting up a digital collection site using [Omeka Classic](https://omeka.org/classic/), and using [Twarc](https://github.com/DocNow/twarc), a command line tool and Python library for collecting twitter data. There is no single tool that will work for everyone's needs, and we hope in the future to provide further documentation in this toolkit on additional resources. 

As part of a planning processes, we recommend exploring tools that you may want to use during a rapidly evolving crisis that requires digital collecting. Our hope is that this toolkit will provide a starting place if you need to get your own site up and running quickly. 

### Omeka for Digital Collections

Omeka offers two platforms -  Omeka Classic and Omeka S - for publishing and managing your digital collections. Our digital collecting site runs on [Omeka Classic](https://omeka.org/classic/), which is at the core of what is currently offered in this toolkit. Follow the materials in our toolkit section on [Setting up Omeka Classic]({{ site.url }}{{ site.baseurl }}/docs/omeka-setup) to build a site similar to [_"Unite the Right" Rally and Community Response_](http://digitalcollecting.lib.virginia.edu/rally/). We've identified [plugins]({{ site.url }}{{ site.baseurl }}/docs/omeka-setup/omeka-plugins) and created a [custom theme]({{ site.url }}{{ site.baseurl }}/docs/omeka-setup/custom-theme) specifically for use with Omeka Classic. 

Your project needs may align instead with [Omeka S](https://omeka.org/s/), which offers many of the same options as Omeka Classic. Instead of plugins, Omeka S provides [modules](https://omeka.org/s/modules/) to extend the functionality of your site. The [Collecting](https://omeka.org/s/modules/Collecting/) module offers the equivalent to the Contribution plugin for collecting public contributions through your site. The [Custom Vocab](https://omeka.org/s/modules/CustomVocab/) module is comparable to the Simple Vocab plugin for providing predetermined vocabulary for any metadata elements. See the complete [User Manual](https://omeka.org/s/docs/user-manual/) for Omeka S, and the complete list of [modules](https://omeka.org/s/modules/) for that platform. Our toolkit offers some materials on setting up an Omeka S site for collecting, [here]({{ site.url }}{{ site.baseurl }}/docs/omeka-s)


### File Size Limitations

You'll want to consider setting a limit on the file size for individual contributions uploaded through your site's collection form. These settings are server specific, and can be set up by your server administrator when you install Omeka. If you're using Reclaim Hosting, or another shared hosting service, you may not be able to change the file size limitations. 

For our digital collecting site, we set the maximum file size for uploads at 250Mb. This is large enough for short video files taken with smartphones, which was an item we were interested in collecting. Creating a limit on file size may seem restrictive, but it is important for the sustainability of your server, where your files are stored. Your available server space is determined by your institution or your shared hosting service (like [Reclaim](https://reclaimhosting.com/)), so consider how much total space you have for file storage when determining size restrictions. 

### Large Files and File Sets

Currently, the Contribution plugin for Omeka Classic allows for only individual file uploads, with a maximum file size set by your server administrator. For our site, we encourage contributors to use the contribution form to submit their materials, as it provides the simplest way for us to process the items we receive. However, for files larger than 250Mb or for large file sets we provide an option for contributing a URL link for an album or file location (i.e. Dropbox folder, Flickr album, etc.). When images and video files are uploaded directly through the contribution form, they're processed as Omeka items, and easily managed from the Omeka dashboard. Materials submitted as links have required significantly more time on our end to include them in the collection, and has been a major impediment to making more of our archive public. 

Omeka offers the Dropbox plugin, which lets Omeka users batch upload a large quantity of files at once. It allows you to upload multiple files directly into a folder on your server that you can then add in the items admin interface. We have not used this plugin at this time for our site, but it offers one option for handling large file set submissions.

- [Dropbox plugin download](https://omeka.org/classic/plugins/Dropbox/)
- [Dropbox plugin User Guide](https://omeka.org/classic/docs/Plugins/Dropbox/)

## Funding Opportunities

This project was made possible in part by a 2018 award from the [Catalyst Fund at LYRASIS](https://www.lyrasis.org/Leadership/Pages/Catalyst-Fund.aspx). It may be worth exploring grant programs that can help support your digital collections.

[Documenting the Now](https://www.docnow.io/) has an annual call for applicants for Community-Based Digital Archives Workshops for Activists. Their workshops focus on helping activists to develop the skills and to use available tools to collect, preserve, and share their web, social media and other types of digital content in their own digital archive.


This page was updated: July 24, 2019
{: .fs-3 }
