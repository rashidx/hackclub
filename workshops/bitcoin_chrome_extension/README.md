---
name: Bitcoin Chrome Extension
description: Build a Chrome extension that displays live Bitcoin prices.
author: "@rashidx"
group: experimental
order: 16
---

# Bitcoin Chrome Extension
Hello there, hacker!

With Bitcoin and other crypto-currencies booming like never before, it's very important that young hackers like you get involved in this revolution. Getting involved can take many forms, from investing, to mining, to even creating a simple chrome extension.

![Bitcoin meme](9)

> If you have no idea what Bitcoin is, we suggest you watch this [short video that explains how Bitcoin works](8).

In this tutorial, we're going to build a Chrome extension that displays live Bitcoin prices using the [Blockchain API](1).

We will be introducing you to the basics of building Chrome extensions and jQuery—a javascript library which you should have been exposed to if you've done the ["That Was Easy"](2) workshop. It is highly recommended that you go through that workshop and the ["Personal Website"](10) workshop, as some basic HTML, CSS, Javascript and jQuery knowledge is required.

##### Pre-requisites
* Basic HTML knowedge
* Some familiarity with Javascript and the jQuery library
* The Google Chrome browser
* A text editor (we recommend [Atom](3))

By the end of this tutorial, you will learn the basic structure of a Chrome extension, how to run and test a Chrome extension, how to fetch data from APIs in Javascript, and how to use the `change` event in jQuery.

**Table of Contents**
- [Part I - Setting Up](#part-i-setting-up)

## Part I: Setting up
### Creating our extension folder
Every chrome extension is contained in a folder. To start, create a folder on your machine called `bitcoin_price_extension`. After that, we need to create a `manifest.json` inside your folder. Copy and paste the following into the file:
```
{
  "manifest_version": 2,
  "name": "Bitcoin Price Checker",
  "version": "1.0"
}
```
We will explain later what each of the values mean. Right now, we have built the most basic version of a chrome extension that one can run.
### Enabling developer mode
In order for us to be able to run and test our chrome extension, we must enable the developer mode in Chrome. To do that, open your chrome menu by clicking the three vertical dots in the top-right corner.

![Opening the Chrome menu](4)

Then, click on `More tools`, followed by `Extension`.

![Clicking on the Extensions after expanding the More Tools menu](5)

You will be taken to the Chrome extensions page. In the top-right corner, set the `Developer Mode` switch to on. If it has been turned on, you should see a menu pop up with `Load Unpacked`. Click that and select your extension folder.

![Selecting extension folder](7)

You should now see your extension on top of the extensions list.

[1]: https://blockchain.info/api
[2]: https://hackclub.com/workshops/that_was_easy
[3]: https://atom.io/
[4]: img/1_chrome_menu.png
[5]: img/2_tools_extensions.png
[6]: img/3_toggle_dev_mode.png
[7]: img/4_select_extension_folder.png
[8]: https://www.youtube.com/watch?v=Gc2en3nHxA4
[9]: img/0_intro_meme.gif
[10]: https://hackclub.com/workshops/personal_website
