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

## Where to Start

### Gathering a Team

### Planning your Site
What are you collecting?

### Ethical Considerations

### Funding Opportunities

Grant programs that can help support your digital collections:

## Technical Considerations

### Omeka for Digital Collections

Omeka offers two platforms -  Omeka Classic and Omeka S - for publishing and managing your digital collections. Our digital collecting site runs on [Omeka Classic](https://omeka.org/classic/){:target="_blank"}, which is at the core of what is currently offered in this toolkit. Follow the materials in our toolkit section on [Setting up Omeka Classic]({{ site.baseurl }}{% link docs/omeka-setup/custom-theme.md %}) to build a site similar to [_"Unite the Right" Rally and Community Response_](http://digitalcollecting.lib.virginia.edu/rally/){:target="_blank"}. We've identified [plugins]({{ site.baseurl }}{% link docs/omeka-setup/omeka-plugins.md %}) and created a [custom theme]({{ site.baseurl }}{% link docs/omeka-setup/custom-theme.md %}) specifically for use with Omeka Classic. 

Your project needs may align instead with [Omeka S](https://omeka.org/s/){:target="_blank"}, which offers many of the same options as Omeka Classic. Instead of plugins, Omeka S provides [modules](https://omeka.org/s/modules/){:target="_blank"} to extend the functionality of your site. The [Collecting](https://omeka.org/s/modules/Collecting/){:target="_blank"} module offers the equivalent to the Contribution plugin for collecting public contributions through your site. The [Custom Vocab](https://omeka.org/s/modules/CustomVocab/){:target="_blank"} module is comparable to the Simple Vocab plugin for providing predetermined vocabulary for any metadata elements. See the complete [User Manuel](https://omeka.org/s/docs/user-manual/){:target="_blank"} for Omeka S, and the complete list of [modules](https://omeka.org/s/modules/){:target="_blank"} for that platform.

### Virus Scanning

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
