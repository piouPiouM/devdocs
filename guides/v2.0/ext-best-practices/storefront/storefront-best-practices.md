---
layout: default
group: ext-best-practices
subgroup: 03_Storefront
title: Storefront UI best practices
menu_title: Storefront
menu_order: 1
menu_node: parent
version: 2.0
github_link: ext-best-practices/storefront/storefront-best-practices.md
---
##{{page.menu_title}}
{:.no_toc}

The storefront theme is the front facing interface for a Magento application that can be customized through a [theme extension]({{page.baseurl}}frontend-dev-guide/themes/theme-general.html). We suggest adopting the following best practices to avoid common problems we have seen other developers make while making a theme extension.

### Clear your cache periodically

Forgetting to clear or disable caching can cause a lot of development headache. Visual spot checks on rendered content are unreliable when the content being displayed is retrieved from the cache. We recommend clearing your cache before doing visual checks for your theme to make sure the content displayed is correct.

You can manage your cache in the Admin section under **System > Cache Management**.

**Recommended Reading**

* [Clear directories during development]({{page.baseurl}}howdoi/php/php_clear-dirs.html)

### Consider different resolutions/devices

When developing your theme extension, you should check how it looks using different resolutions or devices. We recommend you apply [responsive web design(RWD)](https://en.wikipedia.org/wiki/Responsive_web_design){:target="_blank"} concepts to optimize the look and feel of your theme on different devices and resolutions. To help you with this task, both [Chrome](https://developer.chrome.com/devtools){:target="_blank"} and [FireFox](https://developer.mozilla.org/en-US/docs/Tools){:target="_blank"} web browsers have built in developer tools that allow you to view your theme under different resolutions.

**Recommended Reading**

* [How to make your theme responsive and mobile]({{page.baseurl}}frontend-dev-guide/responsive-web-design/rwd_overview.html)

### Inherit and customise

There is a lot of work in building a theme extension for Magento from scratch. This is why we recommend you inherit and customize an existing theme. Magento comes with both Blank and Luma themes after initial install. You can leverage the work already done to make those two themes responsive by setting one of them as your theme's parent.

**Recommended Reading**

* [Theme inheritance]({{page.baseurl}}frontend-dev-guide/themes/theme-inherit.html)
