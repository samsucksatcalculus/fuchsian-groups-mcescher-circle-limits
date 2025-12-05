# fuchsian-groups-escher
This repo contains the Cayley graphs and group presentations of the Fuchsian groups underlying M.C. Eschers Circle Limit artworks. It does not contain any code. If you follow this very brief tutorial, you should be able to read a group presentation off a (Euclidean, hyperbolic or spherical) tesselation.

<div style="display: flex; justify-content: center;">
  <img src="https://github.com/samsucksatcalculus/fuchsian-groups-escher/blob/main/readme/Circle-Limit-I.jpeg?raw=true" 
       alt="Circle Limit 1" 
       style="width: 24%; margin: 1%;">
  <img src="https://github.com/samsucksatcalculus/fuchsian-groups-escher/blob/main/readme/Circle-Limit-II.jpeg?raw=true" 
       alt="Circle Limit 2" 
       style="width: 24%; margin: 1%;">
  <img src="https://github.com/samsucksatcalculus/fuchsian-groups-escher/blob/main/readme/Circle-Limit-III.jpeg?raw=true" 
       alt="Circle Limit 3" 
       style="width: 24%; margin: 1%;">
  <img src="https://github.com/samsucksatcalculus/fuchsian-groups-escher/blob/main/readme/Circle-Limit-IV.jpeg?raw=true" 
       alt="Circle Limit 4" 
       style="width: 24%; margin: 1%;">
</div>

Fuchsian groups are discrete subgroups of the group of orientation preserving isometries of the upper half plane. They act properly discontinuously on the upper half plane and thus give rise to a tesselation. Along the Cayley map $C$ we can pass back and forth between the upper half plane model and the unit disk model of the hyperbolic plane without losing notions of hyperbolic distance.

$$
\begin{align}
  C: \mathbb{D} &\to \mathbb{D} \\
              z &\mapsto \frac{z-i}{z+i}
\end{align}

\begin{align}
  C^{-1}: \mathbb{D} &\to \mathbb{D} \\
              z &\mapsto -i \; \frac{z+1}{z-1}
\end{align}
$$

In general Fuchsian groups have Dirichlet regions, i.e. in particular they have polygonal, convex fundamental domains. In the case of M.C. Eschers Circle Limit, we can find Dirichlet regions which are compact and finite-sided.

By Sabidussis Theorem the Cayley graph of the Fuchsian groups underlying these circle Limits is isomorphic to the dual tiling graph of the tesselations by these compact, finite-sided fundamental polygons. From this Cayley graph we can deduce a set of generators (the transformations which moves an arbitrary but fixed "start-tile" to a tile with which it shares a side). These generators pair the sides of the start-tile in a unique way and thus are called side-pairing transformations. 

For finite sided fundamental polygons its vertex set must be finite as well. The side-pairing transformations partition the vertex set of the fundamental polygon into vertex cycles. These subsets are called vertex cycles because a subset of the side pairing transformations cyclically permutes the elements in each vertex cycle.

Taking the elements (in order) which cyclically permute the vertex cycle, we can derive a relation between them by looking at the sum of the angles at the vertices in the interior of the fundamental polygons. The angle sum for each vertex cycle will always be $\frac{2\pi}{k}$, for some $k \in \mathbb{Z}$.

<p align="center">
     <img src="https://github.com/samsucksatcalculus/fuchsian-groups-escher/blob/main/readme/anglesums.png?raw=true"
          alt="interior angle size and vertex cycles of fundamental polygon of circle limit III"
          width="500">
</p>
