# eventual

[![Build Status](https://secure.travis-ci.org/Gozala/eventual.png)](http://travis-ci.org/Gozala/eventual)

An abstraction for eventual values.

## What is an eventual value?

An eventual value is a placeholder for values that will be
recieved asyncronously *at some point in the future*. Eventual values are typically
used in place of callbacks for asyncronous operations. They allow you to
return a deferred value *syncronously* that will be resolved
*asyncronously*. Using deferred values allows you describe
asyncronous actions in a syncronous fashion.

You may have seen eventual value abstractions before: `jQuery.deferred` and
`Promise` are both abstractions layers for eventual values.

By allowing you to return a future value immediately, eventuals give you
a handy way to avoid nested callback hell. They also make it easy to
describe asyncronous control flows that are difficult to handle with
callbacks ("do this when x and y are ready, then wait for any of a, b
and c, and do that").

## Install

    npm install eventual

