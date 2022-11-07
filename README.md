
# A Chrome extension using JavaScript

In this project, we're going to build a chrome extension by using JavaScript.
Before we start building, it would be great if we could get a sense of what exactly is a Chrome extension and how it works under the hood in a browser. On a basic level, an extension is just a collection of HTML, CSS and JavaScript snippets that lets us execute some extra functionalities through the JavaScript APIs that the Chrome browser exposes. In layman's terms, an extension is mostly a webpage hosted inside Chrome with access to some specific APIs.

 We're going to walk you through creating a basic Chrome extension called CryptoBase. This kind of extension fires a browser notification based on the fulfilment of specific business logic inside our extension and optionally execute some Javascript.

There are also a few terms you'll need to get accustomed to before we begin.

Chrome extensions start with a manifest.json file. You can run code in the background using the background service worker. Any code specific webpage can be run through a content scripts file while the Options file is used to help the users customise the extension by providing an options page by right-clicking the extension icon in the toolbar and finally, the main UI element of our Chrome extension will be built using the popup file.


A step-by-step guide to launching your own Chrome extension using JavaScript.
Step 1: Setting up the initial project.
Step 2: Creating a manifest file.
Step 3: Building the extension.
Step 4: Submitting for review.
Step 5: Publishing the app on the Chrome Web Store.


First things first, we need to create the project and all the files necessary for extension. Let's begin by creating a new directory called CryptoBase. We'll be keeping all our files in this new folder. Chrome does allow us to load and test our extensiona by pointing to a specific folder that contains all the files.
We also need a manifest file for our extension to run as it tells Chrome everything needs to properly load in our Chrome extension. We'll create a blank manifest.json file and put it into the same root folder called CryptoBase that we created earlier.
Next, we'll need an icon for our extension. There are various dimensions you can go for like 16x16px, 32x32px, 48x48px and 128x128pxor go for a single default size to cover all devices.
After that, we need to create a user interface for our extension and for that we'll use the popup files in our extension by creating HTML, CSS and JS files for the popup in our CryptoBase directory.


Now our basic folder structure is done, we can add code to our manifest.json file which describes our extension to the browser. Use the snipper given below:


1. Creating the user interface.

The first step in coding out our Chrome extension is to create the user interface that will get displayed when the extension icon is clicked. For the purpose of being concise, we'll be keeping the user interface very simple. It consists of a header that says "CryptoBase" followed by a list of top 50 cryptocurrencies(according to their respective market capitalization). 

2. Building the logic.

The last thing we need is to implement the logic which should execute every time when the user clicks the extension icon. We'll want to add a basic fetch request to get the required data from the public API. When the extension icon gets clicked, the values will be fetched and corresponding HTML element will be created in the DOM.

3. Submitting for review.
Before publishing our extension to the Chrome Web Store, we need to get it reviewed from Chrome. Here are a few things we need to do to before submitting our extension for review.







