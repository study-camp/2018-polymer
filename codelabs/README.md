# Codelabs and Tutorials

This is a simple index of codelabs/tutorials with functioning code. A high level description of goals and insights is provided for each. Each directory listed may, in turn, have its own README.md to provide more in-depth notes in due course. 

For simplicity, each directory is prefixed (_10_, _20_ or _30_) to identify the Polymer version that was _targeted_ for that project. If an existing project is _migrated_ to a new version, the old version will be deleted (but remain accessible in repo history).

## [Polymer 2.0 Tour](https://www.polymer-project.org/2.0/start/quick-tour)

## Projects

#### [Build an Element Tutorial](https://www.polymer-project.org/2.0/start/first-element/intro) / [code](20-build-an-element/icon-toggle)

Create a simple custom element (button with icon) with an associated UI behavior (pressed, unpressed) and related data binding and custom CSS properties. The example here differs from the tutorial in that it was built using the Polymer CLI scaffold as a starting point (vs. the starter code provided in the documentation)


#### [Build an App Tutorial](https://www.polymer-project.org/2.0/start/toolbox/set-up) / [code](20-build-an-app/my-starter-app)

Creates a app-layout with slide-out drawer (sidebar) and multi-route (navigation) using the [iron-pages](https://www.webcomponents.org/element/PolymerElements/iron-pages) element. The latter is effectively a container associated with multiple children "pages", one of which is selected to be shown at any given time. By binding this selection to the route, we effectively get a single-page app. 

The starter-kit scaffolding automatically provides progressive web apps support (manifest.json, service workers, PRPL pattern lazy loading etc.) -- the lazy loading is achieved by defining related [fragments](https://www.polymer-project.org/2.0/docs/tools/polymer-json#fragments) in _polymer.json_


#### [Build a Google Drive Client](https://codelabs.developers.google.com/codelabs/polymer-drive-client/index.html) / [code](20-build-an-app/google-drive-client)

Inspired by the [_Google NLP From Sheets_](https://bit.ly/nlp-from-sheets) post, I wanted to explore how to build an application that could use Google Forms (to accept inputs), Google Sheets (to store responses) and Google Cloud ML (to analyze insights) -- and potentially have the resulting stored data used to power a simply Polymer-driven application.

As a starting point, this exercise will explore the existing (2016) codelab for Google Drive components, to see if they are still viable with Polymer 2.0. However, I will be using the _starter-kit_ scaffold to replicate that exercise.
