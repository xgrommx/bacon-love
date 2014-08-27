# Loading Spinner

Showing a spinner while performing some async task is a very common pattern in
clientside programming. In this exercise we will look at how this can be
solved by FRP.

## The Problem

Your task will be to create an observable which holds the current visibility
of a spinner. You will be supplied with one observable which is a stream of
clicks and one function that when called will return an observable
representing the result of the async task.

The spinner should only be visible after the button has been clicked and while
waiting for the result of an async operation. It should not be possible to
start the same task multiple times while still waiting for the result.

## Template

```js
// include the Bacon.js library
var Bacon = require('baconjs');

module.exports = function (clicks, startAsyncTask) {
  var spinnerVisibility;

  return spinnerVisibility;
};
```