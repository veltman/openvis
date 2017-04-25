# OpenVisConf 2017 Bibliography

### D3.js shape tweening demos

[Smoother polygon transitions](https://bl.ocks.org/veltman/4d1413aa5fd3bb5af1a806c146870031) - animating between shapes using added bend vertices and optimized winding

[Jigsaw morphing](https://bl.ocks.org/veltman/c582a31d347e04dd75d5331b0074558e) - animating between one shape and many shapes using an overlay grid and polygon clipping

[Triangulation morphing](https://bl.ocks.org/veltman/14b65b88156d4f5772c285ee7d78403b) - animating between one shape and many shapes with triangulation

[Electoral cartograms](http://bl.ocks.org/veltman/c7bfb3d4a3817f7ee0bf2dd19ff058c1)

[North Carolina redistricting](https://bl.ocks.org/veltman/949ce9c1b6f3e54c6e18)

[Curved shape tweening](https://bl.ocks.org/mbostock/3081153) - tweening between a polygon and a circle by decomposing the circle into a corresponding polygon (by Mike Bostock)

[Custom shape tweening](https://bl.ocks.org/alexmacy/06cf037853999219cd82bc79edc4aee6) - animating between different arbitrary shapes (by Alex Macy)

[Superformula tweening](https://bl.ocks.org/mbostock/1020902) - animating between shapes that can be defined by [Superformula](https://en.wikipedia.org/wiki/Superformula) parameters. (by Mike Bostock and Christophe Viau)

### JavaScript tools

[react-svg-morph](https://github.com/gorangajic/react-svg-morph) - utility for morphing between two SVGs in React

[GreenSock MorphSVG plugin](https://greensock.com/morphSVG) - GSAP shape morphing utility (costs money, not open source)

[d3.geo2rect](https://github.com/sebastian-meier/d3.geo2rect) - a plugin for morphing between GeoJSON and a rectangular SVG grid

[d3-interpolate-path](https://github.com/pbeshai/d3-interpolate-path) - a D3 interpolator to interpolate between two unclosed lines, for things like line chart transitions with mismatched data

[Wilderness](https://github.com/colinmeinke/wilderness) - an SVG manipulation and animation library

[reexpress](https://github.com/blendmaster/reexpress) - Beier-Neely image morphing in JavaScript

[earcut](https://github.com/mapbox/earcut) - fast JS polygon triangulation

### Academic papers and algorithm demos

*Note: most of these are full of words and symbols I really didn't understand, I've marked the ones I found relatively readable and engaging with an asterisk (&ast;).*

#### General 2D Morphing

[Tweening Grammars: Deformation Rules for Representing Change between Discrete Geographic Entities](http://www.geocomputation.org/2005/Kim.pdf)* - relatively accessible overview of lots of different morphing approaches and tradeoffs in the context of visualizing geographic changes over time

[Polygon Vertex Set Matching Algorithm for Shapefile Tweening](http://vis.berkeley.edu/courses/cs294-10-fa08/wiki/images/d/d3/Finalpaper_rc_sv.pdf)* - algorithm for matching vertices between two arbitrary polygons, also discusses the treatment of polygons with holes

[2D Polygon Morphing Using the Extended Gaussian Image](http://web.mit.edu/manoli/www/ecimorph/ecimorph.html) - demo and writeup of a way to morph between two convex polygons by matching and interpolating their extended circular images instead of their points

[Morphing between Geometric Shapes Using Straight-Skeleton-Based Interpolation](http://www.cs.technion.ac.il/~barequet/theses/yakersberg-msc-thesis.pdf.gz) - very long master's thesis outlining an approach to interpolating between two polygons using smoothed versions of their straight skeletons

[2-D Shape Blending: An Intrinsic Solution to the Vertex Path Problem](https://pdfs.semanticscholar.org/0937/24a8e28ca3cc218ceb95a03b8ccc9666cb0a.pdf) - an approach to tweening two similar shapes by interpolating their angles and edge lengths instead of their vertices

#### Image morphing

[Feature-Based Image Metamorphosis](http://graphics.cs.cmu.edu/courses/15-463/2004_fall/www/Papers/beier-neely.pdf)&ast; - original paper detailing one of the foundational image morphing algorithms; includes several gratuitous references to the movie *Ghostbusters*

[Snakes: Active Contour Models](http://web.cs.ucla.edu/~dt/papers/ijcv88/ijcv88.pdf) - a 1988 paper outlining a "snake" approach to edge detection and image manipulation

[Transmogrifiers](http://www.transmogrifiers.org/transmogrifiers.pdf)* - an approach to distorting a shape and its contents based on chosen spines

[Four Corner Image Warping](http://www.fmwconcepts.com/imagemagick/bilinearwarp/FourCornerImageWarp2.pdf)* - a friendly introduction into warping an image between two different quadrilateral shapes

[Morphing Using Curves and Shape Interpolation Techniques](http://nishitalab.org/user/nis/cdrom/pg/morphing.pdf) - a rather involved image warping technique that relies on feature curves rather than simple vectors

#### 3D morphing

[Poisson shape interpolation](https://pdfs.semanticscholar.org/e5f1/2b4ec9401885db46c2fae852707e81670639.pdf) - I understood virtually none of this but it does have some amazing diagrams

[Establishing Correspondences by Topological Merging](http://graphicsinterface.org/wp-content/uploads/gi1991-35.pdf) - a 1991 paper outlining an approach to 3D shape transformation that made a surprising amount of sense

[Shape Transformation Using Variational Implicit Functions](http://www.cc.gatech.edu/~turk/my_papers/schange.pdf) - outlines a method for creating a continuous 3D transformation between two 2D shapes (for example, creating a 3D model of someone's kidney from a series of 2D slices)

[Polyhedral Morphing Using Feature-Based Surface Decomposition](http://gamma.cs.unc.edu/3DMORPHING/demos.html) - Some weird morphing demos, including a woman turning into a triceratops and back (the title is "Tracy to Ruby," it's unclear which one is the woman and which one is the triceratops)

[Zoomorphic Design](http://people.sutd.edu.sg/~saikit/projects/zoomorphic/zoomorphic.pdf)* - A pretty wild paper about blending animals and inanimate objects into hybrids like a horse-shaped chair or a dolphin-shaped tricycle, worth skimming for the terrifying renderings

[3D Morphing](http://compbio.mit.edu/publications/I03_Kamvysselis_3Dmorph_97.pdf) - An overview of a few different possible 3D morphing techniques


#### Morphing graphs with triangulation

[Guaranteed intersection-free polygon morphing](http://www.cs.technion.ac.il/~gotsman/AmendedPubl/GuaranteedIntersection/GuaranteedIntersection.pdf) - A triangulation-based algorithm for morphing corresponding polygons without self-intersections; it involves "spiderwebs" and includes a bat morphing into a cattle skull for some reason

[Intersection-Free Morphing of Planar Graphs](http://gmorph.cs.arizona.edu/gd.html) - demos and a paper for an algorithm that smoothly morphs two planar graphs without self-intersections along the way (requires both graphs to have corresponding structures already)

[As-Rigid-As-Possible Shape Interpolation](http://www.cs.tau.ac.il/~dcor/online_papers/papers/arap.pdf) - A method of morphing shapes in terms of their interior triangulations that I mostly didn't understand but shows a penguin turning into a dolphin

[Morphing piecewise linear shapes using convex representation](http://www.cs.technion.ac.il/~vitus/papers/PhDThesis.pdf) - A PhD thesis on triangulation-based morphing techniques that I did not really understand or finish reading (it's 120 pages long)

[Tweening Boundary Curves of Non-simple Immersions of a Disk](http://www.ics.uci.edu/~gopi/SamplePubs/Tweening.pdf) - some sort of triangulation-based algorithm for morphing certain types of self-intersecting shapes, boy did I not understand most of the words in here

#### Statistical shape analysis and Procrustes transformation

[Introduction to Statistical Shape Analysis](https://graphics.stanford.edu/courses/cs164-09-spring/Handouts/paper_shape_spaces_imm403.pdf)*

[Procrustes analysis on Wikipedia](https://en.wikipedia.org/wiki/Procrustes_analysis)*

### Slide marginalia

[FantaMorph sample gallery](http://www.fantamorph.com/samples.html) - a must-see

[WRAL redistricting comparison](http://www.wral.com/how-2-redrawn-districts-could-affect-most-nc-voters/15339226/) by Tyler Dukes

[On Growth and Form](https://archive.org/details/ongrowthform00thom) by D'Arcy Wentworth Thompson

[Courts are Shaking Up House Elections in 2016](https://www.bloomberg.com/politics/graphics/2015-redistricting/) (Bloomberg News) - includes an animated transformation of Florida's 5th District

[2013 Australian Election Results](https://www.theguardian.com/world/datablog/2013/sep/06/better-election-results-map) from The Guardian
