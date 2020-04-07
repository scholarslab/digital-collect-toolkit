---
layout: default
title: Omeka Plugins
parent: Omeka Classic Setup
nav_order: 1
---

# Omeka Plugins
{: .no_toc }

Download and install plugins to extend the basic functionality of your Omeka site: build forms for community contributions, customize the collected metadata in your archive, and other useful options for your digital collecting site.
{: .fs-6 .fw-300 }
Our [Digital Collecting](http://digitalcollecting.lib.virginia.edu/rally/) site includes the following plugins. Links to download for your site are included below, as well as details on how we used the plugins. You may choose which plugins, among others offered by [Omeka](https://omeka.org/classic/plugins/), are most useful for your site.

Please follow the links for related installation and user guides for details on how to set-up and use the individual plugins. For instructions on installing and managing Omeka plugins, see [here](https://omeka.org/classic/docs/Admin/Adding_and_Managing_Plugins/).


Published: April 25, 2019
{: .fs-3 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Guest User
You must upload and install the Guest User plugin before installing and activating the Contribution Plugin.

- [Download Guest User plugin](https://omeka.org/classic/plugins/GuestUser/)
- [Installation and Configuration Guide](https://omeka.org/classic/docs/Plugins/GuestUser/)

## Contribution

- [Download Contribution plugin](https://omeka.org/classic/plugins/Contribution/)
- [Installation & Configuration Guide](https://omeka.org/classic/docs/Plugins/Contribution/)

The Contribution plugin provides a form to collect stories, images, and other files from the public and manage those contributions in your Omeka site as items. Contributors may share and upload content anonymously, and their information will only be available to site administrators. Other plugins can be integrated into the Contribution form, such as Simple Vocab for creating dropdown menu choices, and Geolocation for inviting users to map their submissions or locations.

Installing and configuring the Contribution plugin requires a few steps. Please read through the [Omeka documentation](https://omeka.org/classic/docs/Plugins/Contribution/) carefully.

See the page on [Collecting Community Contributions]({{ site.baseurl }}{% link docs/collecting-materials.md %}) for additional information on our site's [Contribution Terms of Service](http://digitalcollecting.lib.virginia.edu/rally/contribution/terms) and how we configured this plugin for collecting and managing stories, images, and other files from the public.

## Dublin Core Extended

- [Download Dublin Core Extended plugin](https://omeka.org/classic/plugins/DublinCoreExtended/)
- [Documentation](https://omeka.org/classic/docs/Plugins/DublinCoreExtended/)

Dublin Core Extended provides additional metadata elements that you may find useful to collect in your Contribution collection form. We used this plugin specifically for the 'Spatial Coverage' element, which along with the Simple Vocab plugin, allows contributors to submit the location of their contribution.

## Simple Vocab

- [Download Simple Vocab plugin](https://omeka.org/classic/plugins/SimpleVocab/)
- [Configuration & Use Guide](https://omeka.org/classic/docs/Plugins/SimpleVocab/)

Simple Vocab is a useful plugin for providing predetermined vocabulary for any metadata elements. This plugin allows you to create drop-down menus that replace the usual text box for an element. 

We used Simple Vocab to replace the element for "Spatial Coverage" with a list of locations around Charlottesville relevant to the events. When a contributor chooses to fill out the 'Location' input in the collection form, they choose from a drop-down list of predetermined terms, set in the Simple Vocab settings. Once the plugin is installed, you can manage your custom vocabulary by clicking on the 'Simple Vocab' tab on the left-hand menu in your Omeka dashboard:

![Screenshot of Simple Vocab page in Omeka](https://raw.githubusercontent.com/scholarslab/digital-collect-toolkit/master/assets/images/simple-vocab.png) 

## Element Types

- [Download Element Types plugin](https://omeka.org/classic/plugins/ElementTypes/)

Used for standardizing date input for contribution submissions (provides a pop out calendar for date selection in the Contribution form).

## Derivative Images

- [Download Derivative Images plugin](https://omeka.org/classic/plugins/DerivativeImages/)
- [Documentation](https://omeka.org/classic/docs/Plugins/DerivativeImages/)

## Simple Pages

- [Configuration Guide](https://omeka.org/classic/docs/Plugins/SimplePages/)

Used to create our [About the Archive](http://digitalcollecting.lib.virginia.edu/rally/about) page. This plugin is useful for creating additional text rich pages for your site, and comes bundled with your Omeka download.

## Search by Metadata

- [Download Search by Metadata plugin](https://omeka.org/classic/plugins/SearchByMetadata/)
- [Installation and Configuration Guide](https://omeka.org/classic/docs/Plugins/SearchByMetadata/)

The Search by Metadata plugin makes it possible for visitors to your public Omeka site to see a browse page with items that share specific metadata (i.e., all items with 'UVA Rotunda' in the Spatial Coverage field). This plugin works very well with the Simple Vocab plugin for controlling metadata vocabulary. See the related [Omeka documentation](https://omeka.org/classic/docs/Plugins/SearchByMetadata/) for details on configuring this plugin.

## Additional Plugins

We do not currently have the following plugins active on our collecting site, but they may be useful for others.

### Geolocation

- [Download Geolocation plugin](https://omeka.org/classic/plugins/Geolocation/)
- [Configuration Guide](https://omeka.org/classic/docs/Plugins/Geolocation/)

The Geolocation plugin allows you to assign a location to items in your Omeka site. The locations are displayed on maps on individual items page and on a browsable map of all geolocated items, that you can add to your site's primary navigation. This plugin also allows you to add a map to your Contribution form, allowing contributors to select locations on a map to submit with their materials.  

### Exhibit Builder

- [Configuration Guide](https://omeka.org/classic/docs/Plugins/ExhibitBuilder/)

The Exhibit Builder plugin allows you to develop online exhibits, or special web pages, that combine items from your Omeka archive and may include narrative text. You may find it useful for creating exhibit pages out of collected materials. This plugin is included in your downloaded Omeka installation and does not require a separate download.

### Dropbox 

- [Dropbox plugin download](https://omeka.org/classic/plugins/Dropbox/)
- [Dropbox plugin User Guide](https://omeka.org/classic/docs/Plugins/Dropbox/)

The Dropbox plugin allows you to upload multiple files directly into a folder on your server that you can then add in the items admin interface. 