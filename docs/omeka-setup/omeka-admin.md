---
layout: default
title: Omeka Site Administration
parent: Omeka Classic Setup
nav_order: 5
---

# Administering your Omeka Classic Site
{: .no_toc }

Published: April 25, 2019
{: .fs-3 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Managing Users

Manage users by clicking on the Users tab in the top navigation of your Omeka admin dashboard. The Users section gives the site Administrator control over who may access the admin section of the site and what they can do.

### User Levels and Access

Omeka allows you to give different backend users different levels of access to your archive. Read through the following list of actions available to users to determine what works best for your project team members.

All logged in site Super, Admin, Contributor, and Researcher users can view non-public content (items, collections, Simple Pages, Exhibits, etc) on the site.

### Super Users
{: .no_toc }
Can do anything and everything in Omeka.
Supers are the only users with access to the top navigation tabs for Plugins, Appearance, Users, and Settings.

### Admin Users
{: .no_toc }
Admin users do not have access to the tabs for managing plugins, appearance, users, or site settings.
Admin users can:

- Add, edit, tag, and delete items, both their own and created by other users.
- Make items, collections, exhibits, and other content public or not public.
- Make items, collections, exhibits, and other content features or not featured.
- Add, edit, and delete Item Types.
- Add, edit, and delete files.
- Interact with plugins installed and activated by a SuperUser.
- Add, edit, and delete tags.

### Contributor Users
{: .no_toc }
Contributor users have control over their own content but can only view content created by others. They cannot make their own content public. **Contributor Users are different from 'Guest' and 'Contribution anonymous', the user types added when using the Contribution and Guest User plugins. See [below](#guest-users) for details on these user types**. 
Contributor users can:

- add, edit, tag, and delete items which they created.
- cannot make their own items public.
- create their own exhibits from items that are public.

### Researcher Users
{: .no_toc }
Researchers can log in to the admin side of an Omeka site and see the content, but cannot interact with it in any way. They cannot add, edit, delete, or tag any items.

For complete documentation on managing users, see the related page in the Omeka Classic documentation, [here](https://omeka.org/classic/docs/Admin/Users/){:target="_blank"}.

### Guest & 'Contribution Anonymous' Users {#guest-users}
{: .no_toc }

When using the Contribution and Guest User plugins, two additional user types will become available - Guest & 'Contribution Anonymous'. Depending on how you configure these two plugins, when users make submissions through your contribution form, they will potentially have the option of including their email to set up a 'Guest' user account, or they can choose to make their submission anonymous. 

For details on configuring these settings for user contributions, see the related section in [Collecting Materials]({{ site.baseurl }}docs/omeka-setup/collecting-materials#contributor-anonymity-settings).

## Site Security Settings

Access your site's Security Settings by clicking on the 'Settings' tab in the top navigation of your Omeka admin dashboard. Then select the 'Security' tab in the Settings toolbar:

![Screen shot of Security settings bar]({{ site.url }}{{ site.baseurl }}/assets/images/security-settings.png)

Scroll down to the Captcha section. A captcha is a program that can help ensure that only actual people, not spammers or robots, are using public forms on your Omeka site, including the Contribution plugin content submission form.

In order to use reCAPTCHA, you will need to sign up for Captcha key to reduce spam on your site. Sign up by following the link to the google developer's reCaptcha site, provided in the Captcha section (see below screenshot). Once you sign up, you can enter your site and secret keys in their respective fields:

![Screen shot of Security settings bar]({{ site.url }}{{ site.baseurl }}/assets/images/captcha.png)

For more details on reCaptcha settings, see the related [Omeka Documentation](https://omeka.org/classic/docs/Admin/Settings/ReCaptcha/){:target="_blank"}.

For more information on additional site security settings, see [here](https://omeka.org/classic/docs/Admin/Settings/Security_Settings/){:target="_blank"}.

## Customizing Site Navigation

From your Omeka admin dashboard, click on the 'Appearance' option in the top navigation bar. Select the 'Navigation' tab in the Appearance toolbar to see your site's navigation settings.

These settings determine your site's main navigation, see [our site](http://digitalcollecting.lib.virginia.edu/rally/){:target="_blank"} as an example:

![Screen shot of Navigation bar]({{ site.url }}{{ site.baseurl }}/assets/images/nav-bar.png)

1. To change the default label for a navigation link, click on the arrow to its right and change the text under 'Label' (see the screen shot below, with open editor for 'About the Archive'):

    ![Screen shot of Navigation settings]({{ site.url }}{{ site.baseurl }}/assets/images/nav-settings-1.png)

2. Add a link to your navigation bar using the box 'Add a Link to the Navigation'. To create a link for a search page, fill in the 'Label' and 'URL' as seen below, and click the 'Add Link' button:

    ![Screen shot of Navigation settings]({{ site.url }}{{ site.baseurl }}/assets/images/nav-settings-2.png)

    Use this box to add any additional links to your navigation bar as needed. You can include URLs from outside your Omeka site as well. 

3. Select the check box for links you want to appear in you navigation bar. Click and drag the links to change to your preferred order.

    ![Screen shot of Navigation settings]({{ site.url }}{{ site.baseurl }}/assets/images/nav-settings-3.png)

