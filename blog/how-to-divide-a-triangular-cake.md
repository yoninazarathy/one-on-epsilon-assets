The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2017/04/16/How-to-Divide-a-Triangular-Cake-Between-6-People/). We are in the process of moving it to the current location.

<<<<<<< HEAD
# How to Divide a Triangular Cake Between 6 People?

*April 16, 2017*

**Inna Lukyanenko**

<center>
 <img class = "blog-inline-image" src="https://es-app.com/assets/hd7NMX.jpg" alt="drawing" width="250px"/>
</center> 

Look around. Do you see any triangles? Sure you do, triangles are everywhere. To see one you only need three points. I bet that you can see a triangle in your vicinity right now. Perhaps even multiple triangles if you look hard enough. 

 

But hold on. Even though triangles are simple to describe and easy to spot, there are many facts about triangles that are not immediately obvious. For starters, what is a nice way to cut a triangle into smaller pieces?

 

Imagine for example a triangular cake. Something that looks like this:


 

How would you divide such a cake evenly, between, say, 6 people?

For the usual round cake this is pretty straightforward. It is enough to make 3 straight cuts through the center of the cake that divide it into 6 sectors with equal angles (each of 60 degrees):

 


 

What if we ask the same question about our triangular cake? You may answer:

 

"Just like for a circle, make 3 straight cuts through the center."

 

But where is the center of a triangle? Does it even have a “center”?

Fortunately, Euclidean geometry comes to help. It is a beautiful mathematical system described in Euclid’s book “Elements” as early as 300 BC. Based on axioms and formal proofs, it set the standard of mathematics being a rigorous systematic science rather than a collection of disconnected facts.

 

For the moment, let us assume that we live on a plane, so our world and, in particular, all our cakes are 2 dimensional. Alternatively, we can just imagine that we look at them from the top, like in the pictures above.

 

First of all, let us recall some basic facts about lines on a plane. Any two lines either intersect or they are parallel:

 


Now, 3 lines on a plane generally don’t intersect in one point:

 


But it turns out that certain lines associated with any triangle always intersect in one point! Here we consider one such threesome of lines, called medians. A median is a line connecting a vertex of the triangle with the midpoint of the opposite side.


 

As you can see in the picture above, the vertices of the triangle are marked with A, B and C. Then we construct the midpoints D, E and F and connect each of these with the corresponding opposite vertex of the triangle, to obtain the medians AD, BE and CF.

 

As the figure shows, our triangle is now divided into 6 smaller triangles. What about their area? You probably recall that the area of a triangle equals 1/2 of the base times height:


In particular, this implies that

 

A median cuts a triangle into two pieces of the same area.

 

Can you draw a few illustrations of triangles that show this? Notice that depending on your triangle and your choice of vertex from which to draw the median, the two pieces may look different. But they always have the same size. This is guaranteed because they have the same height and equal bases.

 

So now you know how to divide a triangular cake between 2 people. But if you divide it between 6 people, is the area of all the 6 pieces the same? Actually, does the point G in the figure above even exist? Will the three cuts intersect in one point?

Now here is an incredible fact. And in mathematics, if a fact is incredible enough, or non trivial enough, or important enough, it is called a "Theorem".

 

Theorem: The 3 medians of any triangle intersect in one point, G, called the centroid. Furthermore, the medians divide the triangle into 6 triangles of the same area.

 

A theorem is quite a serious thing for mathematicians. You can't just write it down. It requires a proof. Otherwise it is just a belief, a conjecture or a statement that may be considered true by some and false by others. Having a correct proof, ensures that it is true. Nevertheless, if you believe it already and need to urgently split your triangular cake among 6, follow this:

 

To divide any triangular cake fairly among 6 people, make 3 cuts. Each cut going from a vertex to the center of the opposite side. The theorem above guarantees that the cuts will intersect at a single point. Further, even though the six pieces may not have the same shape, they will all have the same size.  

 

To get a better feel for the medians and the centroid, you can also explore this neat interactive Mathifold visualization. The Mathifold project features a growing collection of visualizations that help illustrate both simple and complex mathematical concepts and phenomena.  In the visualization, you can see that no matter how we deform the triangle, the medians always intersect in one point. 

 

So you saw the theorem about cutting cakes. Are you ready for the proof?

Proof. Construct the medians BE and CF. Denote the point of their intersection by G. We want to show that the line through A and G bisects CB. Denote the point of intersection by D.

 

Note now that our triangle is divided into 6 smaller triangles. Denote the areas of these triangles by


 as follows: 


 

Note that GE is a median of AGC and GF is a median of AGB. Thus, we obtain:


The median BE divides ABC into two triangles (CBE and ABE) of the same area. Thus,


Analogously, looking at the median CF we see that


These equations yield: 


In particular, this implies that the 4 areas


are the same. Denote it by S.

 

Now using the formula for the area of a triangle, observe that for any line connecting a vertex of the triangle with a point on the opposite side, the ratio of the areas of the resulting triangles is the same as the ratio of the bases:

 


 

Now, comparing the areas of CAD and BAD we have


 Analogously, comparing the areas of CGD and BGD, we see that


From the last two equations we obtain


This implies that


and using the equations above, also implies that these two areas equal the rest. Hence all six pieces have the same area. Also using the ratio above, CD=DB, so AD is a median as needed. 

 

Q.E.D.

 

The "Q.E.D." is an abbreviation for the Latin phrase "quod erat demonstrandum", or translated to English: "that which was to be demonstrated". You speak Latin, don't you? It is common practice to finish mathematical proofs with Q.E.D. 

Now, let’s come back to our earlier question “Where is the center of a triangle?” We answered this with the centroid, but it turns out that, unlike circles, triangles have at least 4 possible centers!

 

Apart from the centroid, other common centers are the incenter, circumcenter and orthocenter, all of which were known to the Ancient Greeks. If you aren't familiar with these, can you try and guess how they would be defined? We may discuss these in future blog posts.

 

So now we are ready to deal with triangular cakes and we can dream on about other geometric shapes like quadrilaterals, pentagons, hexagons and so on. Such objects are called polygons. And one day we may even dare to move up a dimension and produce some 3D culinary creations. Perhaps something like this:

 

=======
![Blog header image](https://es-app.com/assets/hd7NMX.jpg){.blog-image-header}
>>>>>>> dace7f58bdfaedccdacf6695c44b927d017da404
