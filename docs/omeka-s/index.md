---
layout: default
title: Omeka S Setup
nav_order: 4
# has_children: true
---

# Setting Up Omeka S

If you are interested in using [Omeka S](https://omeka.org/s/) for your digital collecting site, below are some steps to help you get started. 

## Technical Specifications

If you are a member of a university or institution with an accessible IT Department or Digital Content Developers, we recommend reaching out to individuals in your organization with experience setting up Omeka. 

Omeka S has the following server requirements:
- Linux
- Apache (with [AllowOverride](https://httpd.apache.org/docs/2.4/mod/core.html#allowoverride) set to "All" and [mod_rewrite](https://httpd.apache.org/docs/current/mod/mod_rewrite.html) enabled)
- MySQL, minimum version 5.6.4 (or MariaDB, minimum version 10.0.5)
- PHP, minumum version 7.1, with [PDO](https://www.php.net/manual/en/intro.pdo.php), [pdo_mysql](https://www.php.net/manual/en/ref.pdo-mysql.php), and [xml](https://www.php.net/manual/en/intro.xml.php) extensions installed
- Optional, to create thumbnails: ImageMagick version 6.7.5 or greater, the PHP `imagick` extension, or the PHP `gd` extension

See the [Complete Omeka S Installation Guide](https://omeka.org/s/docs/user-manual/install/) for further details.

If you lack access to a server that meets Omeka's basic requirements, or are looking for a **simpler and less technical set-up process**, we recommend [Reclaim Hosting](https://reclaimhosting.com/), a low-cost shared web host offering one-click Omeka installation, with a free domain registration included. Their support staff is easy to reach and their [Community Forum](https://community.reclaimhosting.com/) offers additional resources. 

-  [Reclaim Hosting](https://reclaimhosting.com/)
-  [Installing Omeka S on Reclaim Hosting](https://community.reclaimhosting.com/t/installing-omeka-s-on-reclaim-hosting/1188)
- [Omeka on Reclaim: Community Forum](https://community.reclaimhosting.com/c/docs/omeka)

## Omeka S Modules

One of the primary features of a rapid response digital collecting site is a user-friendly submission form set up to collect photos, videos, stories, website links, audio and other files from the community. Omeka S offers the [Collecting](https://omeka.org/s/docs/user-manual/modules/collecting/), which adds a content submission form to your public collecting site.

When using the Collecting module, contributors may share and upload content anonymously, and their information will only be available to site administrators. All contributions are private by default and require a site administrator to review and make them public on the Omeka site. See our [Terms of Service]({{ site.url }}{{ site.baseurl }}/docs/collecting-materials) page for related content. 

The module can also automatically add a reCAPTCHA box at the bottom of each form to prevent bots from spamming your website. Collecting also offers options for users to create guest accounts that make it easier for one user to submit multiple items.

See more documentation on using the Collecting module, [here](https://omeka.org/s/docs/user-manual/modules/collecting/).

All registered Omeka S modules can be found, [here](https://omeka.org/s/modules/). Listed below are additional modules you may find useful for your collecting site:
- [Custom Vocab](https://omeka.org/s/docs/user-manual/modules/customvocab/)
- [Mapping](https://omeka.org/s/docs/user-manual/modules/mapping/)
- [Metadata Browse](https://omeka.org/s/docs/user-manual/modules/metadatabrowse/)

This page was updated: April 7, 2020
{: .fs-3 }