![](http://f.cl.ly/items/391y4708420P0H001k1G/meteoric.png)

# meteor-ionic

**Alpha - not ready for production**

### Build [Ionic](http://ionicframework.com/) apps in [Meteor](https://www.meteor.com/)!

This is an attempt at **real Ionic and Meteor integration**. This is not just Ionic's CSS framework wrapped in a Meteor package. It aims to be a complete port of [Ionic’s Angular directives](http://ionicframework.com/docs/api/) to [Meteor Blaze](https://www.meteor.com/blaze) templates.

## Why?
[Ionic](http://ionicframework.com/) is probably the most comprehensive, polished, cross-platform mobile framework available. But unfortunately a large portion of its functionality comes from Angular directives. I'm not a fan of trying to force-fit Angular into Meteor, so I wanted to see if I could rewrite Ionic specifically for Meteor. [Here's a blog post I wrote about the similarities between Angular directives and Meteor Templates](https://medium.com/space-camp/your-meteor-app-probably-doesnt-need-angular-13986a0323f6).

## Status

**Not ready!** See the TODO section below to see which Angular Directives have been ported to Blaze.

## Dependencies
Rather than include compiled or CDN versions of Ionic's CSS Framework we’ve extraced it into two separate packages:

- [meteoric:ionicons-sass](http://github.com/meteoric/ionicons-sass) Ionic’s Ionicons set wrapped for Meteor.
- [meteoric:ionic-sass](http://github.com/meteoric/ionic-sass) The base Ionic CSS Framework wrapped for Meteor.

## Examples

### [Meteor Hunt](https://github.com/meteoric/meteorhunt)
A [Product Hunt](http://producthunt.com) clone built in Meteor Ionic.

## TODO

### Angular Directives to convert to Blaze:
* [x] ActionSheet
* [x] Backdrop
* [x] Content
  * [x] ion-content
  * [x] ion-refresher (not necessary with Meteor)
  * [x] ion-pane
* [ ] Events (use a 3rd party library?)
* [x] Form Inputs (using [`meteoric:autoform-ionic`](https://github.com/meteoric/autoform-ionic))
  * [x] ion-checkbox
  * [x] ion-radio
  * [x] ion-toggle
* [ ] Gesture (use a 3rd party library?)
* [x] Headers/Footers
  * [x] ion-header-bar
  * [x] ion-footer-bar
* [ ] Keyboard
* [ ] Lists
  * [ ] ion-list
  * [ ] ion-item
  * [ ] ion-delete-button
  * [ ] ion-reorder-button
  * [ ] ion-option-button
  * [ ] collection-repeat
* [x] Loading
* [x] Modal
* [ ] Navigation (requires iron:router integration)
  * [x] ion-nav-view
  * [x] ion-view
  * [ ] ion-nav-bar
  * [ ] ion-nav-buttons
  * [ ] ion-nav-back-button
  * [ ] nav-clear
* [ ] Platform
* [x] Popover
* [ ] Popup
* [ ] Scroll
  * [ ] ion-scroll
  * [ ] ion-infinite-scroll
* [x] Side Menus
  * [x] ion-side-menus
  * [x] ion-side-menu-content
  * [x] ion-side-menu
  * [ ] expose-aside-when (not sure this is needed)
  * [x] menu-toggle
  * [x] menu-close
* [ ] Slide Box
* [ ] Tabs
  * [x] ion-tabs
  * [ ] ion-tab