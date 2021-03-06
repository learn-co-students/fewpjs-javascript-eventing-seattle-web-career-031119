# How to Leverage JavaScript Events

## Learning Goals

* Define a JavaScript event
* Identify different types of user events

## Introduction

We've experimented with selecting and manipulating nodes in the DOM using
JavaScript: deleting nodes, editing nodes, etc. But most web applications are
_not_ used by people opening up the console and editing the DOM using Chrome's
DevTools :). Instead, people _do something_ and then _work happens_.

"Doing work" in response to "something happening" is known as _event handling_.
_Events_ are the "something that happens" and the "_callback function_" is the
work that will happen in response to the event being triggered. In this lesson
we'll focus on the first half of that relationship: the event. We'll discuss
the second half, the "callback function," or, "callback" in a later lesson.

We'll explore this relationship in this document.

## Define a JavaScript Event

JavaScript has the ability to "listen" for things that happen inside the
browser. It can listen for events like whether the browser resized, or
whether someone clicked on a specific image on the screen. The event you're
probably most familiar with is "click."

We'll cover a few more common types of events below.

## Identify Different Types of User Events

Let's take a look at some of the more common events.

### Mouse Click

The mouse / trackpad is a primary pointing device when working with
browsers. In response to click, double-click, right-click, etc. we
can do work like, changing the background of the document to a random
color every time someone clicks on the page.

### Key Press

While click events make up the majority of events you'll use, the
keyboard is _also_ an important source of events. We can listen
for `keypress`, `keydown`, and `keyup`. When these events are handled,
we can find out which keys were pressed (like if a space was hit to make
the character jump over the hole).

### Form Submission

HTML pages often use a submit button to submit a form to a server. When a user
submits a form, the `submit` event is fired. An event handler here might pop up
a thank you overlay, play a song, or provide some other sort of interactivity 
depending on what values were entered in the form.

### List of Events

As you seek to build more complicated applications, you'll need to handle and
trigger work on more events. Here's a list of a [ton of browser
events][list].


## Conclusion

JavaScript allows us to trigger work when it detects events.  Some other common
events are `scroll`, `mouseenter` and `mouseleave`, `focus`, `blur`,  and
`onchange`. There are lots and lots of events - what events do popular websites handle?
When JavaScript recognizes an event that applies to a "event handler" that has been set
up, it will execute that "handler's" work, which is stored in a _callback function_.
This might feel intimidating at first, but if you familiarize yourself with them all now,
you can get the hang of using them before you end up needing them for a project task!

## Resources

- [MDN - Web Events][MDN]
- [StackOverflow - Bubbling and Capturing][SO]
- [QuirksMode - Event order][QM]

[instructions]: http://help.learn.co/workflow-tips/github/how-to-manually-open-a-lab
[help-center]: http://help.learn.co/the-learn-ide/common-ide-questions/viewing-html-pages-in-the-learn-ide
[MDN]: https://developer.mozilla.org/en-US/docs/Web/Events
[SO]: http://stackoverflow.com/questions/4616694/what-is-event-bubbling-and-capturing
[QM]: http://www.quirksmode.org/js/events_order.html
[list]: http://help.dottoro.com/larrqqck.php
