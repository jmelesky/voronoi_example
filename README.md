# A Voronoi Example

A python3 example of a very, very simple algorithm for generating
Voronoi diagrams, using a few different distance metrics.

Initially developed to help illustrate [a blog post about distance measures](http://phaedrusdeinus.org/posts/2016-08-25-different-distances.html).

# Usage

Fairly straightforward. First, generate a series of random points:

    $ ./generate_points.py

This will create a local file called `cells.dump`, which is a `pickle`
containing a random set of points (x, y coordinates) and a color
associated with each one.

Once that's in place, generate the Voronoi diagram:

    $ ./render_voronoi.py

This generates another file, a PNG, which shows the Voronoi diagram of
the cells in `cells.dump`.

To generate a diagram using a different distance measure, open up
`render_voronoi.py`, and edit the `distance` function to relay to a
different function.

This isn't terribly user-friendly, but it's a bit of a one-off set of
scripts.
