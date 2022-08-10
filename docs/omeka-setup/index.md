---
layout: default
title: Omeka Classic Setup
nav_order: 3
has_children: true
---

# Setting Up Omeka Classic

The University of Virginia Library's Digital Collecting site, [_The University of Virginia Collection on the Events of August 11-13, 2017 in Charlottesville, VA_](http://digitalcollecting.lib.virginia.edu/rally/) runs on [_Omeka Classic_](https://omeka.org/classic/).
{: .fs-6 .fw-300 }

[_Omeka_](omeka.org) is a leading open source collections-based web publishing platform developed by the [Roy Rosenzweig Center for History and New Media](https://rrchnm.org/) and supports a robust open source developer community. Omeka is standards-based, grounded in a flexible [Dublin Core Metadata Schema](https://omeka.org/classic/docs/Content/Working_with_Dublin_Core/). Omeka takes a user-centered, access-focused approach to collections, emphasizing approachable, accessible web design.

## Technical Specifications

If you are a member of a university or institution with an accessible IT Department or Digital Content Developers, we recommend reaching out to individuals in your organization with experience setting up Omeka.

Omeka Classic has the following system requirements:
- Linux operating system
- [Apache](https://www.apache.org/) HTTP server (with `mod_rewrite` enabled)
- [MySQL](https://www.mysql.com/) version 5.0 or greater
- [PHP](https://www.php.net/) scripting language version 5.3.2 or greater (with mysqli and exif extensions installed)
- [ImageMagick](https://www.imagemagick.org/script/index.php) image manipulation software (for resizing images)

If you lack access to a server that meets Omeka's basic requirements, or are looking for a **simpler and less technical set-up process**, we recommend [Reclaim Hosting](https://reclaimhosting.com/), a low-cost shared web host offering one-click Omeka installation, with a free domain registration included. Their support staff is easy to reach and their [Community Forum](https://community.reclaimhosting.com/) offers additional resources.

-  [Reclaim Hosting](https://reclaimhosting.com/)
-  [Installing Omeka Classic on Reclaim Hosting](https://community.reclaimhosting.com/t/installing-omeka-classic-on-reclaim-hosting/193)
- [Uploading Plugins and Themes to Omeka on Reclaim Hosting](https://community.reclaimhosting.com/t/uploading-plugins-to-omeka/195)
- [Working with Omeka Classic on Reclaim Hosting](https://community.reclaimhosting.com/t/working-with-omeka-classic/194)
- [Omeka on Reclaim: Community Forum](https://community.reclaimhosting.com/c/docs/omeka)


Omeka also provides a list of suggestions for low-cost shared web hosts that offer the server environment required for Omeka, see [here](https://omeka.org/classic/docs/GettingStarted/Hosting_Suggestions/) for details.
- [Complete Omeka Classic Installation Guide](https://omeka.org/classic/docs/Installation/Installation/)

## Omeka Classic Plugins

One of the primary features of a rapid response digital collecting site is a user-friendly submission form set up to collect photos, videos, stories, website links, audio and other files from the community. Omeka Classic offers the [Contribution plugin](https://omeka.org/classic/docs/Plugins/Contribution/), which adds a content submission form to your public collecting site.

When using the Contribution plugin, contributors may share and upload content anonymously, and their information will only be available to site administrators. All contributions are private by default and require a site administrator to review and make them public on the Omeka site.

The plugin can also automatically add a reCAPTCHA box at the bottom of each form to prevent bots from spamming your website. Contribution also offers options for users to create guest accounts that make it easier for one user to submit multiple items.

**In addition to the Contribution plugin, there are additional Omeka Classic plugins that may be useful to your digital collecting site. See the following page for details on [Omeka Classic Plugins]({{ site.baseurl }}{% link docs/omeka-setup/omeka-plugins.md %}).**

## Custom Omeka Theme

This toolkit also offers a custom Omeka theme that you can download for the styling and content of your public Omeka site. This is not required, but you may find it useful for getting your collecting site up and running quickly with minimal technical knowledge. Our theme offers customizable settings for the appearance and content of your site, easily accessible from the Omeka admin dashboard, no coding knowledge needed! For details on installing and customizing our Digital Collecting Theme for your site, see [here]({{ site.baseurl }}{% link docs/omeka-setup/custom-theme.md %}).

## Administering your Omeka Classic Site

For helpful information on administering your Omeka Classic site, including managing users, security settings, and site navigation, see the related page in this toolkit: [Omeka Site Administration]({{ site.baseurl }}{% link docs/omeka-setup/omeka-admin.md %}).


This page was published: April 25, 2019
{: .fs-3 }