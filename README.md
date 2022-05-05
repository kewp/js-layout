# js-layout

This library aims to open things up
so that we aren't all stuck with css -
to enable a choice of

 - how structure is described
 - how layout is specified
 - how elements are drawn

so right now on the web we have to
use html to describe the structure.
also, we have to use css for the
layout. and we have to use the dom.

the aim then is to provide an example
of a set of standards that might allow
the swapping out of these parts - what
do we need in each to allow them to
be swappable?

## structure

perhaps here we just have a node,
a node has properies (name/value pairs),
and a node has children...

## layout specification

maybe just a _rule_ and a rule is
applied to a _node_ in the structure.

> it may be a good aim to have a way
> to recreate the standard css behavior,
> for example cascading ... (even although
> this may be what has made css so
> hard to use!). not sure how to enable
> this but i don't want to introduce
> that notion now.

## rendering

so at first we'd just have a dom and
canvas renderer, and we'd pass it a
structure and a layout specifier ...

but the renderer needs to know things -
presumably all it gets are a list of
boxes with width, height ... how do
we specify the border, for example?

> this is about _layout_ so ... how
> do we split out the actually drawing?
> 
also the renderer needs to pass back
the size of the window.

