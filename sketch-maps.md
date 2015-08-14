# Principles of route generalization

The problem is to encode what we usually think of as a human mental operation,
where you have a sense of what it means to get somewhere and what you need to
do to communicate to somebody else how to get there.

The trick is to provide a framework that enable the route follower to move up
and down the ladder of abstraction from high-level orienting schema to
low-level contextual details.

Note that this problem can be decomposed into two distinct sub-problems: 

* orientation: giving the user an overall view of the route to be taken

* guidance: progressively disclosing relevant information based on the user's
  location and context

This is best addressed with two distinct, but linked, view modes:

* the zoomable map

* the scollable sequence (itinerary/timeline)


The most difficult part is the layout.  The aim is to capture the basic outline
of the route as a sketch map.  This involves rescaling certain elements of the
route and eliminating information that isn't essential for the basic
route-following task.  For our particular use case, **we also want to represent
the topography and landscape of the route, appropriately generalized for a given zoom level.**

* Preserve angular orientation of streets at intersections

* Scale down longer segments (but with enough length for labeling)

* Scale up shorter segments and complex intersections

