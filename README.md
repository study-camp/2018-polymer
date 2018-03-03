# 2018-polymer
Exploring Polymer Development in 2018

 * [1. Setup](#1-setup)
 * [2. Scaffolding a Project](#2-scaffolding-a-project)
 * [3. Exploring Codelabs and Tutorials](#3-codelabs-and-tutorials)


<hr/>

## 1. Setup

Currently using [Polymer 2.0](https://www.polymer-project.org/2.0/start/), installed using the process documented [here](https://www.polymer-project.org/2.0/start/install-2-0). 

Also validated install of other dependencies (node, npm, bower). The ideal way to do this is to first install [Node Version Manager (nvm)](https://github.com/creationix/nvm/blob/master/README.md), then use it to install the latest version of Node (and npm), then use _npm_ to install other dependencies (including _polymer-cli_ and _bower_).

```
$ npm install -g polymer-cli
..

$ polymer --version
1.6.0
$ nvm --version
0.33.2
$ node --version
v8.9.4
$ npm --version
5.7.1
$ bower --version
1.8.2
```

**RELEVANT POLYMER 2.0 LINKS**
 
 * [Start](https://www.polymer-project.org/2.0/start/)
 * [Feature Overview](https://www.polymer-project.org/2.0/docs/devguide/feature-overview)
 * [App Toolbox](https://www.polymer-project.org/2.0/toolbox/)
 * [2.0 Docs](https://www.polymer-project.org/2.0/docs/api/)
 * [Blog](https://www.polymer-project.org/blog/)
 * [Shop Case Study](https://www.polymer-project.org/2.0/toolbox/case-study) with [demo](https://shop.polymer-project.org/) & [source](https://github.com/Polymer/shop)
 * [News Case Study](https://www.polymer-project.org/2.0/toolbox/news-case-study) with [customization](https://news-docs.polymer-project.org/), [demo](https://news.polymer-project.org) & [source](https://github.com/Polymer/news)

Note that there are significant changes when you migrate to [Polymer 3.0](https://www.polymer-project.org/blog/2018-01-18-polymer-3-new-preview) including:
  * _replacing_ bower with npm (for managing package dependencies)
  * _replacing_ HTML imports with ES6 modules (for package loading)

We will deal with those changes when Polymer 3.0 is formally released (likely in 2018). The update should provide a [Polymer Modulizer](https://github.com/Polymer/polymer-modulizer) tool that makes the migration frictionless.

<br/>

## 2. Scaffolding a Project

Using **Polymer shop demo** (progressive web app) <br/>

```
$ mkdir example-shop
$ cd $example-shop
$ polymer init
? Which starter template would you like to use? shop

$ polymer serve
info:    Files in this directory are available under the following URLs
      applications: http://127.0.0.1:8081
      reusable components: http://127.0.0.1:8081/components/shop/
```



Using **Polymer starter kit**.<br/>
_Note: This creates a routed multi-page app. The 'reusable components' link will give a 404._

```
$ mkdir example-starter
$ cd $example-starter
$ polymer init? 
Which starter template would you like to use? polymer-2-starter-kit
info:    Running template polymer-2-starter-kit...

$ polymer serve
info:    Files in this directory are available under the following URLs
      applications: http://127.0.0.1:8081
      reusable components: http://127.0.0.1:8081/components/polymer-starter-kit/

```

Using **simple app** template (without starter kit)

```
$ mkdir example-app
$ cd $example-app
$ polymer init
? Which starter template would you like to use? polymer-2-application
info:    Running template polymer-2-application...
? Application name my-site
? Main element name my-site-main
? Brief description of the application A simple personal website 

$ polymer serve
info:    Files in this directory are available under the following URLs
      applications: http://127.0.0.1:8081
      reusable components: 
```

Using **custom element** template

```
$ mkdir example-elem
$ cd $example-elem
$ polymer init? 
? Which starter template would you like to use? polymer-2-element
info:    Running template polymer-2-element...
? Element name about-me
? Brief description of the element Element that displays a business card for the person

$ polymer serve
info:    Files in this directory are available under the following URLs
      applications: http://127.0.0.1:8081
      reusable components: http://127.0.0.1:8081/components/about-me/

```

_The projects do not check in the build/ bower components/ and node modules/ directories. Simply run "bower install" (to install dependencies) and "polymer build" (to build distributions) from code_ 

In due course, each project/codelab folder will contain updated **README.md** files that provide insights/notes to help understand that specific content or code.

<br />

## 3. Codelabs and Tutorials

These are the relevant Polymer 2.0 codelabs.

 1. [Build and Deploy Polymer 2.0 App From Scratch](https://codelabs.developers.google.com/codelabs/whose-flag/index.html)
 2. [PRPL Pattern with Custom Elements and Firebase](https://codelabs.developers.google.com/codelabs/prpl-ce-firebase/index.html)
 3. [Build an Image Carousel Element with Polymer 2.0](https://codelabs.developers.google.com/codelabs/polymer-2-carousel/index.html)
 4. [Image Styling with Web Components](https://codelabs.developers.google.com/codelabs/image-styling-web-components/index.html)
 5. [How to contribute to Web Components Ecosystem](https://codelabs.developers.google.com/codelabs/web-components-how-to-contribute/index.html)
 6. [Build Google Maps using Web Components and no code](https://codelabs.developers.google.com/codelabs/polymer-maps/index.html)
 


Also check out these older codelabs - note they are Polymer 1.0 but I hope to 
"update" them to validate usage with Polymer 2.0

 1. [Interact with Bluetooth devices on the web with Polymer](https://codelabs.developers.google.com/codelabs/polymer-bluetooth/index.html?index=..%2F..%2Findex)
 2. [Build a PWA with Firebase and PolymerFire](https://codelabs.developers.google.com/codelabs/polymer-firebase-pwa/index.html)
 

Additional Tutorials to explore

 1. [Build an Element](https://www.polymer-project.org/2.0/start/first-element/intro) | [Build an App](https://www.polymer-project.org/2.0/start/toolbox/set-up) - the starting point for learning the basics
 2. [Using the News App](https://news-docs.polymer-project.org/docs/using.html) where you can explore and customize the implementation behind the [design](https://www.polymer-project.org/2.0/toolbox/news-case-study)


