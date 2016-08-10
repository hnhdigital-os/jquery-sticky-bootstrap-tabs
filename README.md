jquery-sticky-bootstrap-tabs
=================
[![npm version](https://badge.fury.io/js/jquery-sticky-bootstrap-tabs.svg)](https://badge.fury.io/js/jquery-sticky-bootstrap-tabs)

Provides pushState (back and forward button support) to Bootstrap tabs

Install
=======
NPM
---
type `npm install jquery-sticky-bootstrap-tabs --save` to install the library via NPM

Bower
-----
type `bower install jquery-sticky-bootstrap-tabs --save` to install the library via bower


Usage
=====

Run this in document ready or some equivalent initializer on your page:

    $('.nav-tabs').stickyTabs();

Where `nav-tabs` is the default class for the bootstrap tabs feature.

Options
=======

The following options are available to pass to jquery-sticky-bootstrap-tabs on instantiation

**Example**

````javascript
$(function() {
	var options = { 
		selectorAttribute: "data-target",
		backToTop: true
	};
	$('.nav-tabs').stickyTabs( options );
});
````

|option|default|description|
|------|-------|-----------|
| selectorAttribute | false | Override the default `href` attribute used as selector when you need to activate multiple TabPanels at once with a single Tab using the `data-target` attribute. |
| backToTop |false | Prevent the page from jumping down to the tab content by setting the backToTop setting to true. |
| showParentTabs |false | Show the parent tabs so the selected tab comes into view if it is part of another tab grouping. |
| showTabUsingClickTrigger |false | Activate the requeted tab using the click trigger so that any behaviours on the click trigger are activated. |
