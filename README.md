# 2018-polymer
Exploring Polymer Development in 2018

## 1. Setup

Currently using [Polymer 2.0](https://www.polymer-project.org/2.0/start/), installed using the process documented [here](https://www.polymer-project.org/2.0/start/install-2-0).

```
$ npm install -g polymer-cli
..

$ polymer --version
1.6.0
```

Relevant Polymer 2 links:
 
 * [Start](https://www.polymer-project.org/2.0/start/)
 * [Feature Overview](https://www.polymer-project.org/2.0/docs/devguide/feature-overview)
 * [App Toolbox](https://www.polymer-project.org/2.0/toolbox/)
 * [2.0 Docs](https://www.polymer-project.org/2.0/docs/api/)
 * [Blog](https://www.polymer-project.org/blog/)
 * [Shop Case Study](https://www.polymer-project.org/2.0/toolbox/case-study) with [demo](https://shop.polymer-project.org/) & [source](https://github.com/Polymer/shop)
 * [News Case Study](https://www.polymer-project.org/2.0/toolbox/news-case-study) with [customization](https://news-docs.polymer-project.org/), [demo](https://news.polymer-project.org) & [source](https://github.com/Polymer/news)


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

## 3. About Polymer




