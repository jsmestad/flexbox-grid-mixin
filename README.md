# flexbox-grid-mixin

### Why another grid mixin?

All the solutions out there fell into two categories:

* Did not support flexbox, instead favoring `float: left` solutions
* Required the use of `.col-1-xs` or some other cluttered syntax

What I was after was a way to set my grid **only** using SCSS mixins. This is
similar to how [neat](http://neat.thoughtbot.io) works.


## Features

### "Standard" Grid

What I mean by a "standard grid" here is that in a 12 column configuration, you
can have an incomplete row of columns only occupying > 12 columns. This will
leave a space at the end of the row untouched.

### Flex Grid

Using the flex grid means setting `@include columns(12)` will give a column a
larger `flex` property. It is preferred to use `@include column;` in this
configuration and modifying the `flex-grow` and `flex-shrink` values yourself.


## Copyright

See LICENSE in this repository for details.
