# tarjan.js

## JavaScript implementation of Tarjan's strongly connected components algorithm

[Tarjan's strongly connected components algorithm](https://en.wikipedia.org/wiki/Tarjan%27s_strongly_connected_components_algorithm), published in paper Enumeration of the Elementary Circuits of a Directed Graph by Robert Tarjan in 1972, is a graph theory algorithm for detecting all cycles and loops (edges connecting vertices to themselves) in a directed graph.

It performs a single pass of depth-first search. It maintains a stack of vertices that have been explored by the search but not yet assigned to a component, and calculates "low numbers" of each vertex (an index number of the highest ancestor reachable in one step from a descendant of the vertex) which it uses to determine when a set of vertices should be popped off the stack into a new component.

It is trivial to write algorithms to detect cycles in a graph, but most approaches prove highly impractical due to the immense time and storage they require to complete the computation. Tarjan's algorithm is one of the precious few that is able to compute strongly connected components in linear time (time increases linearly with the number of vertices and edges).
The others include Kosaraju's algorithm and the path-based strong component algorithm (Purdo, Munro, Dijkstra, Cheriyan & Mehlhorn, Gabow). Although Kosaraju's algorithm is conceptually simple, Tarjan's and the path-based algorithm are favoured in practice since they require only one depth-first search rather than two.

This JavaScript implementation of Tarjan's algorithm is based on the [PHP version](https://github.com/Vacilando/php-tarjan) I created in 2015.

## More information and live demo

[https://www.vacilando.org/article/javascript-implementation-tarjans-cycle-detection-algorithm](https://www.vacilando.org/article/javascript-implementation-tarjans-cycle-detection-algorithm)
