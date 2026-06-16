# Notes on DRM/ARM
Note: *All example images will be relative to green in front and white on top*

## Recognition (You can skip this technically, as it's useful for the same side of the scramble you are on, but it's useful to know in case you don't know if the RZP you have is good or not)

### Top Pairs
Most useful metric.  If you only learn one thing, it should be this.

An easy way to visualize a top pair is if an E layer edge is in the U or D layer and a corner is attached to it so that it can make an 'F2L pair'.  A 1x3 bar counts as two pairs, as you can have two pairs sharing the same edge.

![Top pair circled in red](https://drive.google.com/thumbnail?id=1EE8poBZveGaGztIjpPDcJEsopxuqQy6q&sz=w1000)

*Circled is a top pair*

The definition that covers over to both Top pairs and Side pairs is where you have an edge and a corner that are paired up next to each other and can be solved together in 1-2 non-EO breaking moves

### Side Pairs
Side pairs are somewhat useful, but a bit more difficult to locate.  For the side pairs, my brain sees it best by looking for edges that are not in DR, and look for a corner that is not in DR that is in the R/L face.  It should be lined up next to a bad corner that if an R or L is applied, the corner would become a good corner.

![Side pair circled in pink/purple](https://drive.google.com/thumbnail?id=1u-THqGfPLmOy9_JMIUS0L_mWsQ0Z8GkH&sz=w1000)

*Circled is a side pair*

### ARM
To understand ARM, we first need to understand JZP.  A cube is in JZP if we don't need any U/D quarter turns (and EO is solved).  JZP only applies to the U/D layers.  A corner in JZP will have the U/D color facing upwards, forwards, or backwards.  It will not be facing right or left.  The only way for an edge to be out of JZP is when an edge that belongs in the E layer is in the M layer.  You can notate ARM with ar-XcYe where X is the number of non-JZP corners, and Y is the number of non-JZP edges.

![Edge out of JZP](https://drive.google.com/thumbnail?id=1OSS22TeIpuFAeXHXL9JYpDFsb3Fr_HFi&sz=w1000)![Corner out of JZP](https://drive.google.com/thumbnail?id=1QAory0lyBDPCP5HvwTZtZlVJhFrBDJpT&sz=w1000)

*On the left is an edge outside of JZP (add one edge to ARM counting).  On the right is a corner outside of JZP (add one corner to ARM counting)*

## Looking into the inverse
While the above is fundamental to understanding if an RZP is statistically good or bad, what is more useful is to see if applying NISS is useful.  Because of this, we need to learn how to trace each of those categories through NISS

### Top Pairs
To see if we have any top pairs if we NISS, we need to first look for E layer edges that are not in DR.  We will then look for corners which are not in DR that (without counting the U/D colors) contain both colors (again, not counting the color on the U/D face).  You can have a maximum of two matches per non-DR edge in the E layer.

![Inverse Top Pair Edge](https://drive.google.com/thumbnail?id=1JUhgyuCO3AizpEJuenjZkPzaQ5QzIw_V&sz=w1000)![Inverse Top Pair Corner](https://drive.google.com/thumbnail?id=1gqqoejWoPRniNCLIQsks64JFd8fZzHNt&sz=w1000)

*Circled on the left is the inverse's top pair edge.  Circled on the right is the inverse's top pair corner.  Specifically the side colors we look for in the inverse's top pair corner.*

### Side Pairs
To see if we have any side pairs if we NISS, we need to first look for the edges in U/D that are not in DR.  From there, we will look for corners that are not in DR that have the same colors as the edge, but shares the same U or D color that the edge also has in U or D.  For example, if the UF edge has Blue on U and Orange on F, we'd look for the both the White Blue Orange or Yellow Blue Orange corner and count how many have the Blue on U or D faces.

![Inverse Side Pair Edge](https://drive.google.com/thumbnail?id=1YUsYxfVFF-uOa3bA8XP2VN1QDQuPi42e&sz=w1000)![Inverse Side Pair Corner](https://drive.google.com/thumbnail?id=1TVas81IRofqYA_EMn56tdSirWUXSJTY7&sz=w1000)

*Circled on the left is the inverse's side pair edge.  Circled on the right is the inverse's side pair corner, but circled again in yellow to emphasize the U/D color matches.*

### ARM
To get our ARM count, we'll separate it out for edges and corners:

Edges can only add to our ARM count if they are in the E layer.  They add to our ARM count if a bad edge is in the E layer and has an F or B color on the R or L face.

![Inverse ARM Edge](https://drive.google.com/thumbnail?id=1AzUL1xxSDmox3ePYqYmJ13-iU942V3yp&sz=w1000)

Corners add to our ARM count if they have an R or L color on the U or D face.

![Inverse ARM Corner](https://drive.google.com/thumbnail?id=1OHS5IBl4Uv9t93vE1lb5lxEd0JCWe1fb&sz=w1000)

## Applying these counts to determine if we should ARM or not.
For a full in-depth analysis, you can look at [Rodney Kinney's breakdown](https://rodneykinney.github.io//DRM-ARM-stats/drm_trees/), but you can follow specific rules for each RZP to get a low miss-NISS rate.

If any of the following criteria is met, you should also look at NISSing

4e4c
* If you have two or more top pairs
* One top pair with ARM-2c1e
* JZP (ARM-0c0e)

4c2e
* If you have two or more top pairs
* One top pair with one side pair
* JZP (ARM-0c0e)

3c2e
* Always switch